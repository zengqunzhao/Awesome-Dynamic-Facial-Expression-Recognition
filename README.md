# Awesome Dynamic Facial Expression Recognition

**This repo presents the performance of the SOTA methods on popular in-the-wild DFER benchmarks.**<br>
**The superscript # denotes methods conducted with the same Dynamic Sampling, the code can be found [HERE](https://github.com/zengqunzhao/Former-DFER/tree/main/dataloader).**<br>
**Contributions are very welcome! Feel free to pull request and improve this repo!**<br>



- **Content**
  - [DFEW Benchmark [ACM MM 2021]](#dfew-benchmark-acm-mm-2021)
  - [FERV39k Benchmark [CVPR 2022]](#ferv39k-benchmark-cvpr-2022)
    - [Basic DFER](#basic-dfer)
    - [Cross-Scenario Challenge](#cross-scenario-challenge)
  - [MAFW Benchmark [ACM MM 2022]](#mafw-benchmark-acm-mm-2022)
    - [11-Class Uni-Modal Single Expression Classification](#11-class-uni-modal-single-expression-classification)
    - [11-Class Multi-Modal Single Expression Classification](#11-class-multi-modal-single-expression-classification)
  - [CAER Benchmark [ICCV 2021]](#caer-benchmark-iccv-2021)
  - [AFEW Benchmark [IEEE Multimedia 2012]](#afew-benchmark-ieee-multimedia-2012)
  - [Referances](#referances)

## [DFEW Benchmark](https://dfew-dataset.github.io/) [ACM MM 2021]

<table>
<thead>
  <tr>
    <th rowspan="2">Methods</th>
    <th colspan="7">Accuracy of Each Emotion (%)</th>
    <th colspan="2">Metrics (%)</th>
  </tr>
  <tr>
    <th>Happy</th>
    <th>Sad</th>
    <th>Neutral</th>
    <th>Anger</th>
    <th>Surprise</th>
    <th>Disgust</th>
    <th>Fear</th>
    <th>UAR</th>
    <th>WAR</th>
  </tr>
</thead>
<tbody>
  <tr>
    <th>3DR18<sup>#</sup></th>
    <th>76.32</th>
    <th>50.21</th>
    <th>64.18</th>
    <th>62.85</th>
    <th>47.52</th>
    <th>0.00</th>
    <th>24.56</th>
    <th>46.52</th>
    <th>58.27</th>
  </tr>
  <tr>
    <th>R18+LSTM<sup>#</sup></th>
    <th>83.56</th>
    <th>61.56</th>
    <th>68.27</th>
    <th>65.29</th>
    <th>51.26</th>
    <th>0.00</th>
    <th>29.34</th>
    <th>51.32</th>
    <th>63.85</th>
  </tr>
  <tr>
    <th>R18+GRU<sup>#</sup></th>
    <th>82.87</th>
    <th>63.83</th>
    <th>65.06</th>
    <th>68.51</th>
    <th>52.00</th>
    <th>0.86</th>
    <th>30.14</th>
    <th>51.68</th>
    <th>64.02</th>
  </tr>
  <tr>
    <th>EC-STFL<sup>[1]</sup></th>
    <th>79.18</th>
    <th>49.05</th>
    <th>57.85</th>
    <th>60.98</th>
    <th>46.15</th>
    <th>2.76</th>
    <th>21.51</th>
    <th>45.35</th>
    <th>56.51</th>
  </tr>
  <tr>
    <th>Former-DFER<sup>#[2]</sup></th>
    <th>84.05</th>
    <th>62.57</th>
    <th>67.52</th>
    <th>70.03</th>
    <th>56.43</th>
    <th>3.45</th>
    <th>31.78</th>
    <th>53.69</th>
    <th>65.70</th>
  </tr>
  <tr>
    <th>EST<sup>[3]</sup></th>
    <th>86.87</th>
    <th>66.58</th>
    <th>67.18</th>
    <th>71.84</th>
    <th>47.53</th>
    <th>5.52</th>
    <th>28.49</th>
    <th>53.43</th>
    <th>65.85</th>
  </tr>
  <tr>
    <th>STT<sup>#[4]</sup></th>
    <th>87.36</th>
    <th>67.90</th>
    <th>64.97</th>
    <th>71.24</th>
    <th>53.10</th>
    <th>3.49</th>
    <th>34.04</th>
    <th>54.58</th>
    <th>66.65</th>
  </tr>
  <tr>
    <th>NR-DFERNet<sup>#[5]</sup></th>
    <th>88.47</th>
    <th>64.84</th>
    <th>70.03</th>
    <th>75.09</th>
    <th>61.60</th>
    <th>0.00</th>
    <th>19.43</th>
    <th>54.21</th>
    <th>68.19</th>
  </tr>
</tbody>
</table>

## [FERV39k Benchmark](https://wangyanckxx.github.io/Proj_CVPR2022_FERV39k.html) [CVPR 2022]

### Basic DFER

<table>
<thead>
  <tr>
    <th rowspan="2">Methods</th>
    <th colspan="7">Accuracy of Each Emotion (%)</th>
    <th colspan="2">Metrics (%)</th>
  </tr>
  <tr>
    <th>Happy</th>
    <th>Sad</th>
    <th>Neutral</th>
    <th>Anger</th>
    <th>Surprise</th>
    <th>Disgust</th>
    <th>Fear</th>
    <th>UAR</th>
    <th>WAR</th>
  </tr>
</thead>
<tbody>
  <tr>
    <th>C3D</th>
    <th>48.20 </th>
    <th>35.53 </th>
    <th>52.71 </th>
    <th>13.72 </th>
    <th>3.45 </th>
    <th>4.93 </th>
    <th>0.23 </th>
    <th>22.68 </th>
    <th>31.69</th>
  </tr>
  <tr>
    <th>P3D<sup>#</sup></th>
    <th>61.85  </th>
    <th>42.21 </th>
    <th>49.80 </th>
    <th>42.57 </th>
    <th>10.50 </th>
    <th>0.86  </th>
    <th>5.57 </th>
    <th>30.48 </th>
    <th>40.81</th>
  </tr>
  <tr>
    <th>R2Plus1D<sup>#</sup></th>
    <th>59.33 </th>
    <th>42.43 </th>
    <th>50.82 </th>
    <th>42.57 </th>
    <th>16.30 </th>
    <th>4.50 </th>
    <th>4.87 </th>
    <th>31.55 </th>
    <th>41.28</th>
  </tr>
  <tr>
    <th>3DR18</th>
    <th>57.64 </th>
    <th>28.21 </th>
    <th>59.60 </th>
    <th>33.29 </th>
    <th>4.70 </th>
    <th>0.21 </th>
    <th>3.02 </th>
    <th>26.67 </th>
    <th>37.57</th>
  </tr>  
  <tr>
    <th>R18+LSTM</th>
    <th>61.91</th>
    <th>31.95</th>
    <th>61.70 </th>
    <th>45.93 </th>
    <th>14.26 </th>
    <th>0.00 </th>
    <th>0.70 </th>
    <th>30.92 </th>
    <th>42.59</th>
  </tr>
  <tr>
    <th>VGG13+LSTM</th>
    <th>66.26 </th>
    <th>51.26 </th>
    <th>53.22 </th>
    <th>37.93 </th>
    <th>13.64 </th>
    <th>0.43 </th>
    <th>4.18 </th>
    <th>32.42 </th>
    <th>43.37</th>
  </tr>
  <tr>
    <th>Two C3D<sup>[6]</sup></th>
    <th>54.85 </th>
    <th>52.91 </th>
    <th>60.67 </th>
    <th>31.34 </th>
    <th>5.96 </th>
    <th>2.36 </th>
    <th>6.96 </th>
    <th>30.72 </th>
    <th>41.77</th>
  </tr>
  <tr>
    <th>Two R18+LSTM<sup>[6]</sup></th>
    <th>59.00 </th>
    <th>45.87 </th>
    <th>61.90 </th>
    <th>40.15 </th>
    <th>9.87 </th>
    <th>1.71 </th>
    <th>0.46 </th>
    <th>31.28 </th>
    <th>43.2</th>
  </tr>
  <tr>
    <th>Two VGG13+LSTM<sup>[6]</sup></th>
    <th>69.65 </th>
    <th>47.31 </th>
    <th>52.55 </th>
    <th>47.88 </th>
    <th>7.68 </th>
    <th>1.93 </th>
    <th>2.55 </th>
    <th>32.79 </th>
    <th>44.54</th>
  </tr>
  <tr>
    <th>Former-DFER<sup>#[2]</sup></th>
    <th>65.65</th>
    <th>51.33</th>
    <th>56.74</th>
    <th>43.64</th>
    <th>21.94</th>
    <th>8.57</th>
    <th>12.529</th>
    <th>37.20</th>
    <th>46.85</th>
  </tr>
  <tr>
    <th>STT<sup>#[4]</sup></th>
    <th>69.77</th>
    <th>47.81</th>
    <th>59.14</th>
    <th>47.41</th>
    <th>20.22</th>
    <th>10.49</th>
    <th>9.51</th>
    <th>37.76</th>
    <th>48.11</th>
  </tr>
  <tr>
  <th>NR-DFERNet<sup>#[5]</sup></th>
    <th>69.18</th>
    <th>54.77</th>
    <th>51.12</th>
    <th>49.70</th>
    <th>13.17</th>
    <th>0.00</th>
    <th>0.23</th>
    <th>33.99</th>
    <th>45.97</th>
  </tr>
</tbody>
</table>

### Cross-Scenario Challenge

## [MAFW Benchmark](https://mafw-database.github.io/MAFW/) [ACM MM 2022]

### 11-Class Uni-Modal Single Expression Classification

<table>
<thead>
  <tr>
    <th rowspan="2">Models</th>
    <th colspan="11">Accuracy of Each Emotion (%)</th>
    <th colspan="2">Metrics (%)</th>
  </tr>
  <tr>
    <th>AN</th>
    <th>DI</th>
    <th>FE</th>
    <th>HA</th>
    <th>NE</th>
    <th>SA</th>
    <th>SU</th>
    <th>CO</th>
    <th>AX</th>
    <th>HL</th>
    <th>DS</th>
    <th>UAR</th>
    <th>WAR</th>
  </tr>
</thead>
<tbody>
  <tr>
    <th>ResNet18</th>
    <th>45.02</th>
    <th>9.25</th>
    <th>22.51</th>
    <th>70.69</th>
    <th>35.94</th>
    <th>52.25</th>
    <th>39.04</th>
    <th>0.00</th>
    <th>6.67</th>
    <th>0.00</th>
    <th>0.00</th>
    <th>25.58</th>
    <th>36.65</th>
  </tr>
  <tr>
    <th>VIT</th>
    <th>46.03</th>
    <th>18.18</th>
    <th>27.49</th>
    <th>76.89</th>
    <th>50.70</th>
    <th>68.19</th>
    <th>45.13</th>
    <th>1.27</th>
    <th>18.93</th>
    <th>1.53</th>
    <th>1.65</th>
    <th>32.36</th>
    <th>45.04</th>
  </tr>
  <tr>
    <th>EmotionClassifier</th>
    <th>13.60</th>
    <th>4.07</th>
    <th>0.08</th>
    <th>81.09</th>
    <th>75.48</th>
    <th>47.82</th>
    <th>53.02</th>
    <th>-</th>
    <th>-</th>
    <th>-</th>
    <th>-</th>
    <th>39.85</th>
    <th>44.75</th>
  </tr>
  <tr>
    <th>C3D</th>
    <th>51.47</th>
    <th>10.66</th>
    <th>24.66</th>
    <th>70.64</th>
    <th>43.81</th>
    <th>55.04</th>
    <th>46.61</th>
    <th>1.68</th>
    <th>24.34</th>
    <th>5.73</th>
    <th>4.93</th>
    <th>31.17</th>
    <th>42.25</th>
  </tr>
  <tr>
    <th>R18+LSTM</th>
    <th>46.25</th>
    <th>4.70</th>
    <th>25.56</th>
    <th>68.92</th>
    <th>44.99</th>
    <th>51.91</th>
    <th>45.88</th>
    <th>1.69</th>
    <th>15.75</th>
    <th>1.53</th>
    <th>1.65</th>
    <th>28.08</th>
    <th>39.38</th>
  </tr>
  <tr>
    <th>VIT+LSTM</th>
    <th>42.42</th>
    <th>14.58</th>
    <th>35.69</th>
    <th>76.25</th>
    <th>54.48</th>
    <th>68.87</th>
    <th>41.01</th>
    <th>0.00</th>
    <th>24.40</th>
    <th>0.00</th>
    <th>1.65</th>
    <th>32.67</th>
    <th>45.56</th>
  </tr>
  <tr>
    <th>C3D+LSTM</th>
    <th>54.91</th>
    <th>0.47</th>
    <th>9.00</th>
    <th>73.43</th>
    <th>41.39</th>
    <th>64.92</th>
    <th>58.43</th>
    <th>0.00</th>
    <th>24.62</th>
    <th>0.00</th>
    <th>0.00</th>
    <th>29.75</th>
    <th>43.76</th>
  </tr>
  <tr>
    <th>T-ESFL<sup>[7]</sup></th>
    <th>62.70</th>
    <th>2.51</th>
    <th>29.90</th>
    <th>83.82</th>
    <th>61.16</th>
    <th>67.98</th>
    <th>48.50</th>
    <th>0.00</th>
    <th>9.52</th>
    <th>0.00</th>
    <th>0.00</th>
    <th>33.28</th>
    <th>48.18</th>
  </tr>
</tbody>
</table>

**Anger, Disgust, Fear, Happiness, Neutral, Sadness, Surprise, Contempt, Anxiety, Helplessness, Disappointment**

### 11-Class Multi-Modal Single Expression Classification

## [CAER Benchmark](https://caer-dataset.github.io/) [ICCV 2021]

## [AFEW Benchmark](https://cs.anu.edu.au/few/AFEW.html) [IEEE Multimedia 2012]

<table>
<thead>
  <tr>
    <th rowspan="2">Methods</th>
    <th rowspan="2">Pre-trained Datasets</th>
    <th colspan="2">Metrics (%)</th>
  </tr>
  <tr>
    <th>UAR</th>
    <th>WAR</th>
  </tr>
</thead>
<tbody>
  <tr>
    <th>C3D<sup>#</sup></th>
    <th>DFEW (fd1)</th>
    <th>43.75</th>
    <th>46.72</th>
  </tr>
  <tr>
    <th>I3D-RGB<sup>#</sup></th>
    <th>DFEW (fd1)</th>
    <th>41.86</th>
    <th>45.41</th>
  </tr>
  <tr>
    <th>R(2+1)D<sup>#</sup></th>
    <th>DFEW (fd1)</th>
    <th>42.89</th>
    <th>46.19</th>
  </tr>
  <tr>
    <th>3DR18<sup>#</sup></th>
    <th>DFEW (fd1)</th>
    <th>42.14</th>
    <th>45.67</th>
  </tr>
  <tr>
    <th>R18+LSTM<sup>#</sup></th>
    <th>DFEW (fd1)</th>
    <th>43.96</th>
    <th>48.82</th>
  </tr>
  <tr>
    <th>EC-STFL<sup>[1]</sup></th>
    <th>DFEW (fd2)</th>
    <th>\</th>
    <th>53.26</th>
  </tr>
  <tr>
    <th>Former-DFER<sup>#[2]</sup></th>
    <th>DFEW (fd1)</th>
    <th>47.42</th>
    <th>50.92</th>
  </tr>
  <tr>
    <th>EST<sup>[3]</sup></th>
    <th>Unknown</th>
    <th>49.57</th>
    <th>54.26</th>
  </tr>
  <tr>
    <th>STT<sup>#[4]</sup></th>
    <th>DFEW (fd1)</th>
    <th>49.11</th>
    <th>54.23</th>
  </tr>
  <tr>
    <th>NR-DFERNet<sup>#[5]</sup></th>
    <th>DFEW (fd1)</th>
    <th>48.37</th>
    <th>53.54</th>
  </tr>
</tbody>
</table>

## [References]()

1. Jiang X, Zong Y, Zheng W, et al. DFEW: A large-scale database for recognizing dynamic facial expressions in the wild. ACM MM, 2020. [[Paper](https://doi.org/10.1145/3394171.3413620)]
2. Zhao Z, Liu Q. Former-DFER: Dynamic facial expression recognition transformer. ACM MM, 2021. [[Paper](https://doi.org/10.1145/3394171.3413620)] [[Code](https://github.com/zengqunzhao/Former-DFER)]
3. Liu Y, Wang W, Feng C, et al. Expression Snippet Transformer for Robust Video-based Facial Expression Recognition. arXiv, 2021. [[Paper](https://arxiv.org/abs/2109.08409)]
4. Ma F, Sun B, Li S. Spatio-Temporal Transformer for Dynamic Facial Expression Recognition in the Wild. arXiv, 2022. [[Paper](https://arxiv.org/abs/2205.04749)]
5. Li H, Sui M, Zhu Z. NR-DFERNet: Noise-Robust Network for Dynamic Facial Expression Recognition. arXiv, 2022.[[Paper](https://arxiv.org/abs/2206.04975)]
6. Wang Y, Sun Y, Huang Y, et al. FERV39k: A Large-Scale Multi-Scene Dataset for Facial Expression Recognition in Videos. CVPR, 2022.[[Paper](https://arxiv.org/abs/2203.09463)]
7. Liu Y, Dai W, Feng C, et al. MAFW: A Large-scale, Multi-modal, Compound Affective Database for Dynamic Facial Expression Recognition in the Wild. ACM MM, 2022. [[Paper](https://mafw-database.github.io/MAFW/)]
