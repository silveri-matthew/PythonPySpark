<h1>Python - PySpark</h1>


<h2>Description</h2>
Imported a CSV file. Cleaned up the filed and used PySpark package to run a logistic regression.
<br />


<h2>Methods Used</h2>

- <b>PySpark</b>
- <b>Logistic Regression</b>
- <b>Data Cleansing </b>
- <b>Dummy Coding</b> 
  
<h2>Materials Used </h2>

- <b>Jupyter Notebook</b>
- <b>CSV file</b>

<h2>Project walk-through:</h2>

<p align="center">
Data Loading: <br/>
<img src="https://imgur.com/9j1o5LR.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/PyBmtbj.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/F1ahOld.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/QrV7mf0.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/NzJbKhK.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/bmceJ3u.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
Data Cleansing:  <br/>
<img src="https://imgur.com/kNWYePS.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/Xo7EypL.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
Simple Descriptive Statistics:  <br/>
<img src="https://imgur.com/YBeTbRL.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/6WzBGr5.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/PljKTRR.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
Data Recording:  <br/>
<img src="https://imgur.com/LOvdxtC.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/yaFJyAe.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/Lyy0pqT.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/o9nCtX7.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
Modeling:  <br/>
<img src="https://imgur.com/wqsHEaS.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/O3zMVai.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/dTJAkd5.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/ASWlxxL.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/znHcuq8.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/ztsjmr7.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/bgqeQES.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/pUihwwz.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/n7IA7oV.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/BKyuulc.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/4zFfs5C.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/22OmfS4.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/LgpePo3.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/zS629ua.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/frxuBaJ.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/vCSXwbg.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/7tH6vxi.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/H0zCQ2G.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/MxkeWIx.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/vFXpJQw.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<img src="https://imgur.com/O9DWEUe.png" height="80%" width="80%" alt="Project walk-through"/>
<br />
<br />
<p align="left">
<br />
My model's accuracy was 0.973, which is pretty high and indicates that it can correctly predict outcomes in 97.3% of situations. This is particularly significant for default prediction, as accurately identifying situations where a default is likely to occur can be essential for risk management.
The model is doing reasonably well at differentiating between the positive and negative classes, according to the ROC score of 0.961. In order to reduce the frequency of false positives—cases in which the model predicts a default when there isn't one—this is crucial for predicting defaults as well.
The recall and precision scores, however, imply that the model might be constrained in its ability to spot instances of default. With a recall score of 0.997 for the first class (default), the model is successfully detecting the majority of the real positive instances of default. The model is not accurately recognizing many of the actual positive occurrences where a default is unlikely to occur because the recall score for the second class (not default) is relatively low at 0.281. The first class's precision score is similarly quite high, at 0.976, indicating that the majority of the optimistic default forecasts were accurate. The model is producing some incorrect positive predictions for situations where a default is not likely to occur, as evidenced by the precision score for the second class being just 0.75.

Overall, the model's accuracy and ROC score are good, but further analysis and further fine-tuning may be required to enhance the model's performance in predicting occurrences of not default.
Given this situation, the recall and precision scores indicate that the model does a good job of identifying situations in which there is no default but struggles to correctly identify situations in which there is one. This might be a problem if one of the model's key use cases is correctly detecting defaults.

<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
