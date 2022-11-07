Several things that we need to do right now:
    1. Now that we have calculated how many times each category(ICD 10) would appear in one's medical record, now we can do some analysis on that.



Things we will need to do in the future:
    1. 
        1.1 Let X = all people
        1.2 Let Y = all dead people
            1.2.1 Y={B: Dead people caused by other reasons, C: Suicided people}
        1.3 Let Z = all living people

        P(C|Y)+P(B|Y) = 1; ---> 
        P(Y)+P(Z) = P(X)
        We can get P(C/Y): the chance of a dead people who died from suicide. P(B/Y): the chance of a dead people who died from suicide.
        Then we can infer that P(C/Y) \aprox P(C/X),but then how do we do that? If so, why isn't P(C/Y) \aprox P(C/Z)?