# Shallow Optical Flow Three-Stream CNN For Macro and Micro-Expression Spotting From Long Videos



## Reproduce the results for SOFTNet approach (with python script)

<b>Step 1)</b> Download datasets, CAS(ME)<sup>2</sup> (CASME_sq) and SAMM Long Videos (SAMMLV) and placed in the structure as follows:
>├─SOFNet_Weights <br>
>├─Utils <br>
>├─extraction_preprocess.py <br>
>├─load_images.py <br>
>├─load_label.py <br>
>├─main.py <br>
>├─requirements.txt <br>
>├─training.py <br>
>├─CASME_sq <br>
>>├─CAS(ME)^2code_final.xlsx <br>
>>├─cropped <br>
>>├─rawpic <br>
>>├─rawvideo <br>
>>└─selectedpic <br>

>├─SAMMLV <br>
>>├─SAMM_longvideos <br>
>>└─SAMM_LongVideos_V1_Release.xlsx <br>

<b>Step 2)</b> Installation of packages using pip

``` pip install -r requirements.txt ```
<!--
<b>Step 3)</b> Dataset setting

Open main.py, change the dataset name and expression type for evaluation.
-->
<b>Step 3)</b> SOFTNet Training and Evaluation

``` python main.py ```

#### Note for parameter settings <br>
&nbsp; --dataset_name (CASME_sq or SAMMLV) <br>
&nbsp; --expression_type (micro-expression or macro-expression) <br>
&nbsp; --train (True or False) <br>
&nbsp; --show_plot (True or False) <br>





## Guide to run it 
First, you need install the requirements.txt as mentioned, however in any case any library cause ImportError just 
```pip install <that library name>```
Next, dlib library is bit tricky, you need cmake for it. Best way which works is: 
```pip install cmake```
```conda install -c conda-forge dlib```

Finally, I dont recomment you to use Ubuntu as there is a library
```pywin==227```
which is for Window only. 

This may or may not affect result, still checking it out. 
