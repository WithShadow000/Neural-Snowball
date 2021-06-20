# Neural-Snowball
A tensorflow framework for few-shot chinese NRE based on AAAI2020 Paper Neural Snowball for Few-Shot Relation Learning
All the data used are chinese from 



self.generate_candidate_set() 
Use Baidu search to find sentences with the same entity pair

self.generate_data()
Generate training data

self.train()
Generate training data using a random sampling method with the same proportion of positive and negative samples

self.predict_on_data()
Prediction of the unlabeled dataset using RC and RSN to obtain the next pair of entities to be remotely supervised

self.eval(label)
Testing the relation classifier on an unlabeled dataset

self.Candidate_Set :pd.DataFrame
Use Baidu search to find sentences with the same entity pair and calculate a score with RSN

self.data_to_predict :pd.DataFrame
the colnumn 'determined' means the sample have been predicted to be positive
