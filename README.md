# NLP-guide

<h2>NLP Steps</h2>
<ol>
<h3><li>Data Gathering</li></h3>
<ul><li>Make network request to get data</li><li>Beautiful soup (parse HTML docs/extract parts of a website)</li><li>Pickle (Saving python data)</li></ul>
<h3><li>Data cleaning</li></h3>
<ul>
<li><b>Goal</b>: Get the data in a clean, standard format for further analysis</li>
<li>Remove punctuation</li><li>Remove numbers</li><li>Lowercase letters</li>
<li>Remove stop words (words that have very little meaning e.g. the, that). After removing stop words, the text becomes "bag of words model", the order of words doesn't really
 matter.</li><li>Put the words into document-term matrix
 <p>
 <table>
 <tr><th>Comedian</th><th>right</th><th>petunia</th><th>wish</th><th>me</th><th>luck</th>
 <th>die</th><th>august</th><th>hello</th><th>thank</th><th>welcome</th><th>wow</th><th>exciting</th></tr>
 
 <tr><td>John Mulaney</td>
 <td>1</td><td>1</td><td>1</td><td>1</td><td>1</td><td>1</td><td>1</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td>
 </tr>
 <tr><td>Ali Wong</td>
 <td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>3</td><td>2</td><td>0</td><td>0</td><td>0</td>
 </tr>
 <tr><td>Dave Chappelle</td>
 <td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>3</td><td>0</td><td>1</td><td>1</td>
 </tr>
 <tr><td>...</td>
 <td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td>
 </tr>
 </table></p>
 <p>
 Can use scikit-learn - countVectorizer, to create the document-term matrix
 </p>
 </li>
 <li>Corpus (Collection of text)
 <p>
 <table>
 <tr><th>Comodian</th><th>Transcript</th></tr>
 <tr><td>Ali Wong</td><td>Hi, Hello!Welcome! Thank you! Thank you for coming. Hello! Hello.</td></tr>
 <tr><td>Dave Chappelle</td><td>Thank you!Thank you very much!Thank you all. Oh, wow. That was exciting.</td></tr>
 <tr><td>John Mulaney</td><td>All right, Petunia. Wish me luck out there. You will die on Augest 7th, 2037.</td></tr>
 <tr><td>...</td><td></td></tr>
 </table>
 </p>
 </li>
 <li>For implementation, please go to <a href="https://github.com/KeithGalli/sklearn/blob/master/Tutorial.ipynb">https://github.com/KeithGalli/sklearn/blob/master/Tutorial.ipynb</a><ul><li>It includes the steps like data preparing, bag of words vectorization, classifier types (such as svm, decision tree, naive baynes, logistic regression), model evaluation (such as mean accuracy, f1 score for each sentiment), grid search for tunning model parameters and model saving and loading using pickle</li></ul></li>
</ul>
</ol>
