#####ZAP Proxy Integration with Seleniim Driver####
1. Clone this project

2. Add the following dependencies:

    2.1 Inatll ZAP application 
        docker run -u zap -p 8080:8080 -p 8090:8090 -i owasp/zap2docker-stable zap-webswing.sh
        http://localhost:8080/zap
        make sure API key is disabled
        make sure local application is copied
        
    2.2. Install Local application for pen testing
        docker pull psiinon/bodgeit
        docker run --rm -p 8080:8080 -i -t psiinon/bodgeit
        http://localhost:8080/bodgeit
        
3. Run the JUNIT tests
