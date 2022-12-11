# Several things that we need to do right now:
    1. Now that we have calculated how many times each category(ICD 10) would appear in one's medical record, now we can do some analysis on that.



# Things we will need to do in the future:
## 1. Infer to all people
    Let X = all people
        1.2 Let Y = all dead people
            1.2.1 Y={B: Dead people caused by other reasons, C: Suicided people}
        1.3 Let Z = all living people

        P(C|Y)+P(B|Y) = 1; ---> 
        P(Y)+P(Z) = P(X)
        We can get P(C/Y): the chance of a dead people who died from suicide. P(B/Y): the chance of a dead people who died from suicide.
        Then we can infer that P(C/Y) \aprox P(C/X),but then how do we do that? If so, why isn't P(C/Y) \aprox P(C/Z)?


## create a table: 
sex - male female
suicide| yes no
## 2. Model Selection

### 2.1 Linear Model
### 2.2 Non-linear Model
## 3. Matthew’s Correlation Coefficient
    In our case, we should lower the False Negative Rate(FNR) as much as we can.

# Result and Insights
## 1. 看一看到底是年龄呢？还是其他的什么feature更加能让machine learning predictive.
# Note on Nov. 28
### 1. bring additional features to those not able to be seperated.

### 2. Cohen's Kappa Measure.


# Note on Nov. 30

## 1. Giving we have the performance matrix, we want to bring in one more concept: the desire of generalized predicted performance.
### Model Selection/Feature Selection/Hyper-parameters Selection --> Morphism, Feature and Hyper-parameters tuning.

#### 1. Infomation criteria Approach
Goodness of fit Vs. Complexity
Goodness of fit: in training
Complexity: in model

Inductive principle 在学习的过程中一直在发挥影响作用




##### 1. AIC

##### 2. BIC/SIC
##### 3. MDL

#### 2. Randomization Approach

最好的方法去研究哪条路最好的时候，可以采样。 随机采样。

我现在知道了今天我是怎么做的，那我们怎么知道明天会怎样？
我训练了这个set在us，现在我们要用这个训练好的去在eu.

每次我在fraction的时候，feature space会变化。

如果要truly estimate的话，Randomization 啥啥啥的


重复的Nested cross-validation


# 对于随机森林这个东西（超参数数量大于1的时候), 我们就需要随机采样这些possible values了。

有个dataset i.i.d, 我们可以分成若干个batch

[1][2][3][4][5][6]

## 1. For a given morphism f/X;4
[1T][2T][3T][4T][5T][6V]

    Pickup my training dataset
    [1T][2T][3T][4T][5V]
    前四个set是train，最后一个set用来Validate

不停地shuffle 不同的features，可以来找给出最好的训练效果的特征。


不能随便shuffle时间序列，如果要交叉验证的话，那么需要training data是时间order的。




## 1. Training features might leak infomation:

### 1. I: Certain infectious and parasitic disease.

### 2. II: Neoplasms

### 3. IV: Endocrine, nutritional and metabolic diseases.

### 4. IX: Diseases of the circulatory system.(We probably need to drop this.)

### 5. X: Diseases of the respiratory system.(We probably need to drop this.)

### 6. XI: Diseases of the digestive system

### 7. XIV: Diseases of the genitourinary system.


### 8. XVIII: Symtoms, signs and abnormal clinical and laboratory findings, not elsewhere classified.

### 9. XIX: Injury, poisoning and certain other consequences of external causes(We must remove this)
### 10. XX: External causes of morbidity and mortality(We must remove this)



# Note on Dec 5:
## randomization: estimate "generalized" prediction performance
### 1. Classification.
1. MCC
2. AUC
3. ACC
4. Recall

#### 2. Regression.
1. MSE
2. MAE


# Randomnization:
Since learning tasks are nested
-> Nested randomization 'Nested CV'
2 levels: If task 2 and 3 are combined
3 levels: if tasks are learned seperately. 



Nested randomization(CV) for learning:



# Note on Dec 7:

Sequential learning : 每个morphism都是独立的


X_pp ~ h(x,∂;ß)
X_DT ~ δ(X_pp,η;ε)
y ~ f(X_DT,θ;ψ)

y~f(δ(h(x,a;ß),η;ε),theta,)



# Cross Validation
# Hyperpara Search
