# feature validation
> 该部分用于在建模前进行特征检验

## 特殊字符检验

## 重复id/samples

## 特征矩阵稀疏性

### 纵项稀疏性

### 横向稀疏性
类别型特征缺失值处理

连续型特征缺失值处理

## 特征合理性

## 特征与label

|特征类别|target类别|方法                |
|-------|---------|--------------------|
|离散型  |离散型    |chi2                |
|离散型  |连续型    |ANOVA;T-test; IV; KS|
|连续型  |连续型    |correlation family; Mutual Information |

## 特征共线性

### colinearity
> 特征两两之间的共线性

Correlation Matrix

### Multicolinearity
> 多个特征之间的共线性

Variance Inflation Factor

## 特征的时序有效性
PSI


# feature engineering
> 该部分用于将包含较少信息量的原始数据转化为包含更多信息的特征数据，注意特征转换是需要考虑模型算法的，不同模型适合不同的特征

## Binning

### unsupervised
等宽

等频

### supervised
ChiMerge

## encoding
Dummy

WOE

## feature engineering pipeline
define your own feature transformation object which can be embedded in sklearn's pipeline
