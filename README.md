# fmri_nf
## mock dataset demo
since out data is confidential, we provide code to create a mock dataset - containing all the data one needs to run out network, only with random instead of real measured values.
### steps
**create mock dataset**
	```bash
	python3.6 create_mock_data.py --n_subjects <n_subjects>
	```
	This will create a "healthy" subjects dataset, with n_subjects subjects.

**run the e2e training + testing**

	```bash
	python3.6 e2e_train.py --lr <f_learning_rate> --batch_size <f_batch_size> --epochs <f_epochs> --classification_epochs <classification_epochs> --	classifier_lr <classifier_learning_rate> --classifier_batch_size <classifier_batch_size> --type healthy
	```
