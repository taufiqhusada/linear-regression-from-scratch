# Linear Regression from Scratch
Tugas Seleksi Ca-IRK 2018

Membuat algoritma linear regression dari 0.

## Author
Taufiq Husada Daryanto<br>
NIM: 13518058

## Deskripsi Persoalan
Seperti yang telah kalian pelajari pada mata kuliah Probabilitas dan Statistika, terdapat suatu algoritma yang bernama <b>Regresi Linier (Linear Regression)</b>. Buatlah algoritma Regresi Linear versi kalian sendiri dan cobalah memakai algoritma tersebut untuk memproses dataset!

## Dasar Teori Regresi
Regresi linear adalah suatu pendekatan yang memodelkan hubungan antara variabel terikat Y dengan satu atau lebih variabel bebas X. Sehingga, dengan menggunakan regresi linier, kita bisa memprediksi nilai variabel Y dengan menggunakan variabel X.<br>
Regresi linier memiliki persamaan sebagai berikut <br>
<img src="https://render.githubusercontent.com/render/math?math=\hat{Y} = \theta_0 %2B \theta_1 X_i %2B ... %2B \theta_1 X_n"> <br>
dimana: <br>
<img src="https://render.githubusercontent.com/render/math?math=\hat{Y}">: predicted value<br>
n: jumlah feature nya <br>
<img src="https://render.githubusercontent.com/render/math?math=X_i">: value dari feature nya<br>
<img src="https://render.githubusercontent.com/render/math?math=\theta_i">: weight dari featurenya<br>
<img src="https://render.githubusercontent.com/render/math?math=\theta_0">: bias<br>
<br>
Untuk mencari nilai <img src="https://render.githubusercontent.com/render/math?math=\theta"> bisa dengan menggunakan normal equation sebagai berikut
<img src="https://eli.thegreenplace.net/images/math/20baabd9d33dcd26003bc44c7d81ba39e1ad4caa.png" alt="normal-equation-img">
yang pembuktiannya bisa dilihat dari artikel ini https://eli.thegreenplace.net/2014/derivation-of-the-normal-equation-for-linear-regression

## Penjelasan Kode Sumber
Implementasi class LinearRegression ada di file mylib.py <br>
cara penggunaanya sebagai berikut <br>

`from mylib import MyLinearRegression` <br>
`myLinearRegression = new MyLinearRegression()` <br>
`myLinearRegression.fit(X_train, y_train)`        # fit training dataset <br>
`myLinearRegression.predict(X_test)`              # predict test dataset <br>


## References
1. O'Reilly., Hands-on Machine Learning with Scikit-Learn, Keras & TensorFlow
2. https://eli.thegreenplace.net/2014/derivation-of-the-normal-equation-for-linear-regression
3. https://www.kaggle.com/nehalbirla/vehicle-dataset-from-cardekho
