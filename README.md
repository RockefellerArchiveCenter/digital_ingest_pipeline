# digital_ingest_pipeline
Pipeline for ingesting digitized and born digital records into preservation systems.

## Usage

This repository is intended to be deployed in AWS infrastructure.

To provision, authenticate as a user with the necessary permissions, 
update variables and run the following command:

aws cloudformation deploy \
	--template-file digital_ingest_pipeline_template.yaml \
	--stack-name digital-ingest-pipeline \
	--capabilities CAPABILITY_AUTO_EXPAND CAPABILITY_NAMED_IAM \
	--parameter-overrides \
		ArchivesSpacePassword={password for archivesspace user} \

## License

This code is released under the MIT License.