# Datasets-for-automatic-modeling

##Dataset for fine-tuning

The dataset for fine-tuning LLMs consists of instances of objective descriptions and constraint descriptions as well as their annotated type labels. The training set contains 464 descriptions, and the validation set contains 110 descriptions.

Each instance of NL4Opt dataset has a paragraph describing an LP problem. We deconstructed the 99 problem descriptions from the NL4Opt (development) dataset, and obtained 391 descriptions of objectives and constraints. Each problem description has only one objective function. These 292 constraints can be covered by nine types, i.e., types 1 to 9 in the following table. However, the problems in the original NL4Opt dataset do not involve logic constraints. To extend the decomposed NL4Opt dataset, we create a total of 183 descriptions of logic constraints involving two binary variables belonging to four types, i.e. types 10 to 13. 

| Type No. | Type name                                                                        |
|----------|----------------------------------------------------------------------------------|
| 0        | Objective function                                                               |
| 1        | Upper bound on single variable                                                   |
| 2        | Upper bound on sum of variables                                                  |
| 3        | Upper bound on weighted sum of variables                                         |
| 4        | Upper bound on proportion                                                        |
| 5        | Lower bound on single variable                                                   |
| 6        | Lower bound on sum of variables                                                  |
| 7        | Lower bound on weighted sum of variables                                         |
| 8        | Lower bound on proportion                                                        |
| 9        | Comparison constraints                                                           |
| 10       | If A then B/ if not B then not A/ B if A                                         |
| 11       | Exactly one of A and B/ either A or B but not both (or neither)                  |
| 12       | At least one of A and B/ if not A then B/ either A or B or both                  |
| 13       | At most one of A and B/ if A then not B/ either A or B or neither (but not both) |
