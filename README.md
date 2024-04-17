# Mix Marketing Analysis
![Example Image](https://channelmix.com/wp-content/uploads/2019/07/marketing-analyst-1024x717.png)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ekasetyo090/marketing-mix-analysis/blob/master/Mix_Marketing_Modeling.ipynb)

## <div class="header2">📌 Notebook Objectives</div>
<div class="explain-box">
    This notebook <b>aims</b> to:
    <ul>
        <li>Perform <mark>initial data exploration</mark>.</li>
        <li>Perform <mark> data pre-processing using Pandas and its related libraries</mark>.</li>
        <li>Perform <mark> EDA and hypothesis testing</mark> in cleaned dataset.</li>
        <li>Perform <mark> feature engineering </mark>.</li>
        <li>Perform <mark> build RNN predicting model </mark>.</li>
    </ul>
</div>
## <div class="header2">🧾 Dataset Description</div>
<div class="explain-box">
    The following is the <b>structure of the dataset</b>.<br>
<table style="font-family: Inconsolata; font-weight: 300; font-size: 12px; text-align: left; padding: 8px; border-collapse: collapse; width: 100%;">
    <thead>
        <tr>
            <th style="font-family: Inconsolata; font-weight: 900; text-align: center; font-size: 14px; background-color: #C4ECFF">Variable Name</th>
            <th style="font-family: Inconsolata; font-weight: 900; text-align: center; font-size: 14px; background-color: #C4ECFF">Description</th>
            <th style="font-family: Inconsolata; font-weight: 900; text-align: center; font-size: 14px; background-color: #C4ECFF">Sample Data</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><b>TV Manufacturing Brand</b></td>
            <td>TV Manufacturing Brand Name</td>
            <td>TV Manufacturing & Supplier Unit; TV Manufacturing & Supplier Unit ...</td>
        </tr>
        <tr>
            <td><b>DATE</b></td>
            <td>Date of recording</td>
            <td>01/01/2010; 01/02/2010; ...</td>
        </tr>
        <tr>
            <td><b>DEMAND </b></td>
            <td>Product unit demanded</td>
            <td>4384; 4366; ...</td>
        </tr>
        <tr>
            <td><b>Consumer Price Index (CPI)</b></td>
            <td>indexes that measure the average change in price over time for a market basket of consumer goods and services in china.</td>
            <td>104,9; 105,4; ...</td>
        </tr>
        <tr>
            <td><b>Consumer Confidence Index(CCI)</b></td>
            <td>indexes that measures how optimistic or pessimistic consumers are about the economy, labor market, and their spending and financial position.</td>
            <td>96,3; 96,5; ...</td>
        </tr>
        <tr>
            <td><b>Producer Price Index (PPI)</b></td>
            <td>indexes that measure the average change in selling prices received by domestic producers of goods and services.</td>
            <td>106,7; 103,5; ...</td>
        </tr>
        <tr>
            <td><b>Unit Price ($)</b></td>
            <td>Unit Price ($)</td>
            <td>361,62; 400,1; ...</td>
        </tr>
        <tr>
            <td><b>POS/ Supply Data</b></td>
            <td>Product supply unit</td>
            <td>4240; 4266; ...</td>
        </tr>
        <tr>
            <td><b>SALES ($)</b></td>
            <td>Product revenue</td>
            <td>1533268,8; 1542670,92; ...</td>
        </tr>
        <tr>
            <td><b>Advertising Expenses (SMS)</b></td>
            <td>Advertising spend on mobile mesage (SMS)</td>
            <td>77,4819; 73,4783; ...</td>
        </tr>
        <tr>
            <td><b>Advertising Expenses(Newspaper ads)</b></td>
            <td>Advertising spend on newspaper ads</td>
            <td>14,104193; 13,298758; ...</td>
        </tr>
        <tr>
            <td><b>Advertising Expenses(Radio)</b></td>
            <td>Advertising spend on radio</td>
            <td>112,337; 105,7133; ...</td>
        </tr>
        <tr>
            <td><b>Advertising Expenses(TV)</b></td>
            <td>Advertising spend on TV</td>
            <td>1479,4565; 1369,8913; ...</td>
        </tr>
        <tr>
            <td><b>Advertising Expenses(Internet)</b></td>
            <td>Advertising spend on internet</td>
            <td>722,571; 717,857; ...</td>
        </tr>
        <tr>
            <td><b>GRP (NewPaper ads)</b></td>
            <td>gross rating point of newspaper</td>
            <td>95,333; 114,957; ...</td>
        </tr>
        <tr>
            <td><b>GRP(SMS)</b></td>
            <td>gross rating point of SMS</td>
            <td>11,8398; 27,8039; ...</td>
        </tr>
        <tr>
            <td><b>GRP(Radio)</b></td>
            <td>gross rating point of radio</td>
            <td>91; 111,9091;  ...</td>
        </tr>
        <tr>
            <td><b>GRP(Internet)</b></td>
            <td>gross rating point of internet</td>
            <td>276,3636; 291,3182; ...</td>
        </tr>
        <tr>
            <td><b>GRP(TV)</b></td>
            <td>gross rating point of TV</td>
            <td>756,5909; 860,1364; ...</td>
        </tr>
    </tbody>
</table>
<hr>
<center>
    <span class="thanks-watermark">Follow me in other platform: <a href="https://taplink.cc/ekasetyo">https://taplink.cc/ekasetyo_</a></span><br>
    <span class="three-dots2">...</span><br>
    <span class="thanks-watermark"><u>Support me!</u></span><br>
    <span class="trakteer">
        <a href='https://trakteer.id/eka-agung-090' target='_blank'><img src=https://cdn.trakteer.id/images/embed/trbtn-red-1.png?date=18-11-2023" height="40" alt='Support me on trakteer Button'/></a><br>
    </span>
</center>
<hr>
</div>
