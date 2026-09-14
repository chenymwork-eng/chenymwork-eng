# From Predictions to Decisions
**Bayesian reasoning · Model evaluation · AI adoption**

A set of completed analytical case studies exploring when a model output is useful for a decision. The scenarios are exercises, not deployed client systems or empirical field studies.

## Work completed

| Question | Analysis | Decision relevance |
| --- | --- | --- |
| How does evidence change a prediction? | Built a Bayesian network in Python with pyAgrum, learned parameters from a supplied 50-record dataset and examined conditional probabilities. | Make assumptions and the reasoning path explicit. |
| Which classification threshold is appropriate? | Compared confusion matrices and ROC trade-offs at thresholds 0.1, 0.5, 0.7 and 0.9. | Consider false-positive and false-negative costs instead of defaulting to a single accuracy score. |
| Does an association justify an intervention? | Examined confounding and the distinction between observing and intervening. | State what assumptions are needed before using a model to answer a “what if” question. |
| Why might a strong model go unused? | Analysed switching cost, workflow integration, interpretability and alignment with user decisions. | Translate technical performance into requirements for adoption. |
| Can local optimisation create system risk? | Analysed a routing scenario where many users following individual recommendations create congestion. | Evaluate feedback and interactions at system level. |
| How should uncertainty inform action? | Worked with influence diagrams and expected utility. | Make preferences and consequences part of decision support. |

## Example: a threshold is a decision choice

The supplied classification exercise contained 20 cases. At threshold 0.5, the reported confusion matrix had **9 true positives, 8 true negatives, 2 false positives and 1 false negative**, giving sensitivity 0.90 and specificity 0.80.

That balance looked useful in the exercise, but a business threshold cannot be selected from this small example alone. It depends on error costs, base rates and validation on representative data.

## My perspective
Accuracy is an input to a decision, not a substitute for understanding it. An analyst needs to connect model behaviour, uncertainty, user workflows and the consequences of being wrong.

## Scope
These are educational analytical exercises. Causal interpretations depend on the validity of the assumed graph and identification conditions; a Bayesian network alone does not establish causality. No production deployment or measured business uplift is claimed.

**Python · pyAgrum · Bayesian networks · Data reasoning · ROC analysis · Expected utility · AI adoption**
