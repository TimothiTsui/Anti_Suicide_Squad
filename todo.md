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
