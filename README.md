# Supplementary Experiments
### *NeurIPS 2022 Conference Paper4010*

## **1. The time step extended results**

Figure. 1 shows the time step extended result of Humanoid-v2.

<div align=center>
<img src="./Figure1.png"  alt="The time step extended result of Humanoid-v2" width="500" height="450">
</div>


## **2. The challenging explore task results**

Figure. 2 shows the challenging explore task results.

![](Figure2.png "The challenging explore task results")

## **3. The statistical reliability of results**

Figure. 3 shows the statistical reliability of results with IQM metric.

<div align=center>
<img src="./Figure3.png"  alt="The statistical reliability of results with IQM metric" width="450" height="400">
</div>


## **4. The reward noise task results**

Figure. 4 shows the reward noise task results.

![](Figure4.png "The reward noise task results")

The reward noise has an effect on HOER, but only in the early stages. This is due to the fact that the agent may not receive very different rewards early in the training process, which could cause HOER to mistakenly add noisy samples to the ho-buffer as guiding samples, as in walker2d prior to 0.5M. However, it is important to note that HOER will not intervene with exploration. When the cumulative noise return has no effect on the better trajectory, the ho-buffer is gradually updated to the correct better sample, resulting in significant performance gains, as seen in walker2d after 0.5M.

Figure. 5 shows the results of HOER with different noises on Ant-v2.

<div align=center>
<img src="./Figure5.png"  alt="The results of HOER with different noises on Ant-v2" width="450" height="400">
</div>


## **5. The results of HOER_im compared with DisCor**

Figure. 6 shows the results of HOER_im compared with DisCor.

![](Figure6.png "The results of HOER_im compared with DisCor")
