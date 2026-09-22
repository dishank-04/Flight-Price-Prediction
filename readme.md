1) Working of fit_tranform() method

  Working of transform in it -> Say we say SimpleImpute(strategy='median') it will find median of column and save it, no change in raw matrix. Same with OneHotEncode() and OrdinalEncode() they will save details but will not make changes to raw matrix 
  
  now comes working of fit -> The data saved from transform stage will now be applied to raw matrix converting it into design matrix. 

  <h4> WE ALWAYS USE fit_transform() WITH X_train ONLY !!! </h4>

2) Working of tranform() method 
  We apply this to validation set X_val or test dataset X_test it uses the data saved from X_train and apply it to columns of X_val or X_test. 

