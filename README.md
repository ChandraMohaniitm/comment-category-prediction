# Comment Category Prediction Challenge

### This project focuses on building a multi-class classification model to predict how an online platform categorizes user-generated comments. Using a combination of textual data, engagement signals (upvotes/downvotes), emoticon indicators, and topic-related flags, we apply machine learning techniques to accurately determine the final label assigned to each comment.

kaggle competition link : https://www.kaggle.com/code/chandra24208/23f3001092-notebook-t12026/

Techstack: numpy,pandas,matplotlib,seaborn,sckit-learn

<h2>Dataset Overview</h2>

<table border="1" cellpadding="8" cellspacing="0">
  <tr>
    <th>Feature Name</th>
    <th>Data Type</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>comment</td>
    <td>Text (String)</td>
    <td>Raw textual content of the user comment</td>
  </tr>
  <tr>
    <td>created_date</td>
    <td>DateTime</td>
    <td>Date and time when the comment was posted</td>
  </tr>
  <tr>
    <td>post_id</td>
    <td>Categorical / String</td>
    <td>Unique identifier linking the comment to a discussion thread</td>
  </tr>
  <tr>
    <td>emoticon_1</td>
    <td>Binary (0/1)</td>
    <td>Indicator for presence of first emoticon group</td>
  </tr>
  <tr>
    <td>emoticon_2</td>
    <td>Binary (0/1)</td>
    <td>Indicator for presence of second emoticon group</td>
  </tr>
  <tr>
    <td>emoticon_3</td>
    <td>Binary (0/1)</td>
    <td>Indicator for presence of third emoticon group</td>
  </tr>
  <tr>
    <td>upvote</td>
    <td>Integer</td>
    <td>Number of positive reactions received</td>
  </tr>
  <tr>
    <td>downvote</td>
    <td>Integer</td>
    <td>Number of negative reactions received</td>
  </tr>
  <tr>
    <td>if_1</td>
    <td>Numeric (Integer/Float)</td>
    <td>Internal platform feature (hidden meaning)</td>
  </tr>
  <tr>
    <td>if_2</td>
    <td>Numeric (Integer/Float)</td>
    <td>Second internal platform feature (hidden meaning)</td>
  </tr>
  <tr>
    <td>race</td>
    <td>Binary (0/1)</td>
    <td>Indicates reference to race-related topic</td>
  </tr>
  <tr>
    <td>religion</td>
    <td>Binary (0/1)</td>
    <td>Indicates reference to religion-related topic</td>
  </tr>
  <tr>
    <td>gender</td>
    <td>Binary (0/1)</td>
    <td>Indicates reference to gender-related topic</td>
  </tr>
  <tr>
    <td>disability</td>
    <td>Binary (0/1)</td>
    <td>Indicates reference to disability-related topic</td>
  </tr>
  <tr>
    <td>label</td>
    <td>Categorical (Target - 4 Classes)</td>
    <td>Final category assigned to the comment (Only in train dataset)</td>
  </tr>
</table>


<h2>Top Performing Models</h2>

<table>
    <tr>
        <th>Model</th>
        <th>F1 Score</th>
    </tr>
    <tr>
        <td>LGBM</td>
        <td>0.81</td>
    </tr>
        <tr>
        <td>LR</td>
        <td>0.76</td>
    </tr>
        <tr>
        <td>SVC</td>
        <td>0.74</td>
    </tr>
    
</table>
