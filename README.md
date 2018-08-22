## Logistic Regression

### 1 简介  
本项目主要对不同数据集进行特征工程，然后训练不同分类模型对数据进行拟合，包括logistic回归和SVM，最终用于预测。  
- **特征工程**   
  数据探索和数据预处理，具体包括各数据含义解析、数据可视化、数据归一化标准化、特征相关性探索、特征剔除、特征合并、缺失值处理、离群点检测等   
- **分类模型**  
  在处理好的数据集上建立不同的分类模型进行训练，包括使用logistic回归，并探索最佳正则函数（L1/L2）及正则参数，使用线性SVM，并选择最佳参数，使用RBF核的SVM，并选择最佳超参数（正则参数、RBF核函数宽度等）   

### 2 工具包  
数据处理工具包   
- NumPy  
- SciPy  
- Pandas  
  
数据可视化工具包   
- Matplotlib  
- Seaborn  
  
机器学习工具包    
- Scikit Learn  

### 3 数据集介绍  
#### Kaggle2015——Otto Group Product Classification Challenge    
该数据来自Kaggle 2015年举办的Otto Group Product Classification Challenge竞赛数据。Otto数据集是著名电商Otto提供的一个多类商品分类问题，类别数=9. 每个样本有93维数值型特征（整数，表示某种事件发生的次数，已经进行过脱敏处理）。
竞赛官网：https://www.kaggle.com/c/otto-group-product-classification-challenge/data   
第一名：https://www.kaggle.com/c/otto-group-product-classification-challenge/discussion/14335  
第二名：http://blog.kaggle.com/2015/06/09/otto-product-classification-winners-interview-2nd-place-alexander-guschin/    

#### Kaggle2017——Rental Listing Inquiries     
该数据集来自Kaggle 2017年举办的Rental Listing Inquiries分类竞赛数据，需要根据公寓的特征来预测其受欢迎程度（用户感兴趣程度分为高、中、低三类）。其中房屋的特征x共有14维，响应值y为用户对该公寓的感兴趣程度。评价标准为logloss。  
数据链接：https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries  
数据分析示例：https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries/kernels  
竞赛官网：https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries/data   

#### Pima Indians Diabetes Data Set（皮马印第安人糖尿病数据集）    
数据集相对简单，只有一个文件（diabetes.csv）：Pima Indians Diabetes Dataset 包括根据医疗记录的比马印第安人5年内糖尿病的发病情况，这是一个两类分类问题。每个类的样本数目数量不均等。一共有768个样本，每个样本有8个输入变量和1个输出变量。  
