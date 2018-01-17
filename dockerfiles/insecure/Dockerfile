FROM websphere-liberty:webProfile7
MAINTAINER IBM Java engineering at IBM Cloud
COPY server.xml /config/server.xml
COPY com.ibm.apm.dataCollector-7.4.esa /opt/
# Install required features if not present
RUN installUtility install --acceptLicense defaultServer && installUtility install --acceptLicense /opt/com.ibm.apm.dataCollector-7.4.esa
COPY target/microservice-schedule-1.0.0-SNAPSHOT.war /config/apps/schedule.war
