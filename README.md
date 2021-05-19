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

