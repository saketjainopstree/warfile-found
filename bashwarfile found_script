#!/bin/bash
WAR_PATH="/var/lib/jenkins/workspace/build_artifact_job/Spring3HibernateApp/target"

if [[ -f ${WAR_PATH}/Spring3HibernateApp.war ]] ;
then
	echo "Build Completed ....  WAR FileFound !!!!"
	find . -type f -iname "Spring3HibernateApp.war"  | xargs cp -t ../deploy_job/
else
	echo "WAR File not found"
	exit 1
fi
