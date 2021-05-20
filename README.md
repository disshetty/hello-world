# hello-world
Learn new things and trying out different methods
I am new to this platform hope in learning new things and get hold things as soon as possible  
# Day 9

Data pre-processing (Data cleaning)

1.Remove Id because it has no significance
'''
data.drop('Id',axis='columns',inplace=True)



'''
Data analysis (EDA) Visualization

1.COUNTPLOT
Check the the number of values in target
Library: seaborn
Plot   : countplot()
'''
import seaborn as sb
sb.countplot(data['Species'])

'''
2.BOX AND WHISKER PLOT
Plots on the dataframe
'''
data.plot(kind='box',figsize=(10,10))

#3333333333333333
''
Create the arrays
Data- X,Y
dataframe[rows,columns]
'''
x=data.iloc[:,:-1].values
y=data.iloc[:,-1].values

'''
Split the universal dataset
Library : sklearn
Module  : model_selection
Class   : train_test_split
'''
from sklearn.model_selection import train_test_split as tts
x_train,x_test,y_train,y_test=tts(x,y,test_size=0.2,random_state=56)

'''
Selection of Algorithm
ML - SL - Classification
(Categorical target values)
i)LogisticRegression

Library : sklearn
Module  : linear_model
Class  
