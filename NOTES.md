# Quick run
1. Set zone and project
	```
	gcloud config set compute/zone us-east1-c
	gcloud config set project distributed-tf-192015
	```
2. Go to cloudml-dist-mnist-example folder
3. Launch start-training.sh
	```
	MNIST_BUCKET="mnist-31361"
	./scripts/start-training.sh gs://${MNIST_BUCKET}
	```
	
> If required, run ssh-agent:

	```
	eval $(ssh-agent -s)
	ssh-add ~/.ssh/google_compute_engine
	```