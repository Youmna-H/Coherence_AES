This file explains the format of the combined dataset
File format for data (train/dev splits are taken from Taghipour and Ng (2016)):
Each line represents an essay in the format:
essay-id question-id score essay

Essays could be either original or shuffled (each original essay has 4 permutations):

1) original essays do not contain '_' in their essay-id

2) In the shuffled essays essay-id = idOfTheirOriginalEssay_PermutationId, where PermutationId \in [1,4]  and the score field also contains _ but ignore and consider it 0 (the number that comes after '_' is the perm-index from the synthetic_data in the other folder)


Also in the essay, sentence boundaries are marked with $SENTENCE_END$ and the sentences are tokenized with white spaces.
