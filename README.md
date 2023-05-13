# PortfolioAnalysis
This is Python code for analysis of a portfolio model of value chains and similarly networked chains of transmitted values.

Imagine a value chain where raw ingredients go into simple products, and then those products are integrated into more complex products, which then get integrated into even more complex prducts, and so on. This could be a porfolio of ingredients that go into a restaurant menu, or construction materials that go into fabricating machines or building, or financial products that roll up into a nested value chain. This modeling technique calculates how value is transmitted from the simplest raw materials up the levels of complexity in the value chain.

Learn more about the math behind this at https://www.prioritysystem.com/reasons4i.html

According to Priority Systems,

The term "weights" refers to the wi factors in the additive form of a multi-attribute value function [1]:

V(x1,x2...xN) = w1V1(x1) + w2V2(x2) ... + wNVN(xN)	Eq.1
The use of this term may contribute to the common misunderstanding that the wi factors define the relative importance of the objectives and their corresponding performance measures. If, for example, an organization designs a multi-criteria prioritization model with a weight on public safety that is half as large as the weight assigned to net revenue, observers may assume the organization regards public safety as being half as important as profits. The relative value of weights does not support such a conclusion. As shown below, in addition to the relative value attributed to obtaining improvements in performance measures, weights depend on the ranges defined for their assessment [2]. Even though conclusions about the meaning of weights are often based on misconceptions, the fact that such misunderstandings can easily arise underscores the need for taking care when designing the model and when explaining its logic.

Weights as Scaling Factors
As described previously, it is customary to scale (normalize) single-attribute value functions Vi(xi) to go from zero to one [3]. The single attribute value function Vi(xi) converts performance relative to the i'th objective into the relative value of that level of performance. Regardless of the shape of the Vi(xi) functions, the values assigned to the worst and best performance levels are zero and one, respectively.

As indicated by the form of Equation 1, the wi weights serve as scaling factors that allow numbers indicating the relative preference for the performance levels obtained from the single-attribute value functions to be compared with one another and summed [4]. If, for example, performance measure xA has a weight wA that is twice the weight wB for measure xB, then this should be interpreted as meaning that the decision maker values an increment of 0.1 value points on performance measure xA, the same as a 0.2 value point increment for performance measure xB. The wi weights control the sensitivity of total value to changes in the various areas of performance represented in the model. If wi is made smaller, changes in the levels of performance xi will have less significance for determining total value. Conversely, it wi is made larger, total value will be made more sensitive to projects that impact performance in this area.

Weights as Swing Weights
Scaling the multi-attribute value function V( · ) and the single-attribute value functions Vi(xi) in the normal way means that, if xi– and xi+ are the worst and best outcome levels for the i'th performance measure, respectively, and if x– and x+ are the worst and best outcome bundles, respectively, then:

Vi(xi–) = 0 , Vi(xi+) = 1,  i = 1, 2, ..., N
V(x–) = 0 , V(x+) = 1
With this normalization, the weights must sum to one:

Additive value function	Eq.2
Now suppose there are two outcome bundles denoted x1 and x2 that are identical for every measure except the i'th. The i'th measures for the two bundles are set equal the worst and best outcomes for that measure, respectively. The performance levels for the measures other than the i'th, designated x#, are at arbitrary levels but are the same for each bundle (the levels can differ from measure to measure, but whatever the levels are for one bundle they are at the same levels for the second bundle), Expressing these assumption mathematically:

x1 = [xi = xi–;   xk = x#;   k ≠ i]
x2 = [xi = xi+;   xk = x#;   k ≠ i]
With the definitions as given, going from x1 to x2 is the swing from the worst to best outcome for the i'th performance measure (other performance measures remaining unchanged). The value increase associated with this swing is:

V(x2) - V(x1)  =  wiVi(xi+) - wiVi(xi–)  =  wi
This result shows that each scaling factor wi has a very specific interpretation; namely, wi is the relative value (value expressed on a zero to one scale) of obtaining a swing from the worst to best outcome on the i'th performance measure [5]. For this reason, weights are more precisely termed swing weights; they may be obtained by estimating the value of swings from worst to best outcome levels for the performance measures. 