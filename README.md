# Gainforest: Bioacoustic Classification for Amazon and Manaus Bird Species
<p align="center">
  <img src="https://ai.ethz.ch/_jcr_content/orgbox/image.imageformat.logo.1864120785.png" alt="AI ETH Zurich Logo" width="200"  style="margin-right: 30px;" />
  <img src="https://biodivx.org/images/0592ae8160ba0cc72ec64838bb27a1d4.png" alt="BiodivX Logo" width="200"/>
  
</p>
<h1> Model - Wav2vec2 </h1>
<p align="center">
<img src="https://mohitmayank.com/a_lazy_data_science_guide/imgs/audio_wav2vec2_arch.png" alt="BiodivX Logo" width="600"/>
</p>
<h1> Model - Metrics </h1>
<ul> 
 <li> Validation score: ROC-AUC Score (one-vs-rest) </li>
 <li> Training (backpropagation) loss: Weighted cross entropy  </li>
</ul>
<h1> Model - Performance </h1>
<p align="center">
<img src="./assets/training.png" alt="BiodivX Logo" width="600"/>
</p>

<h1> Huggingface Workflow (Gradio) </h1>
<p align="center">
<img src="./assets/poster.drawio (3).png" alt="BiodivX Logo" width="600"/>
</p>
<ul>
<li> <span style="color:blue">  User Inputs (Blue)</span> User selects the model to use, uploads an audio file and chooses the time interval of interest.  </li>
<li> <span style="color:green"> Processing (Green)</span> Audio class and bird species are inference using the model. Model inference results, waveform and mel-spectrogram of the audio are displayed. </li>
<li>  <span style="color:red"> Bird Gallery (Red)</span>  Picture of the predicted bird species are displayed for better understanding the inference result. The picture of birds were fetched via the ebird API. </li>
</ul>