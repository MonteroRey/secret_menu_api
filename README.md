# curl 
curl -v http://localhost:8082/spring-rest/foos/9
curl -d 'id=9&name=baeldung' http://localhost:8082/spring-rest/foos/new
curl -d @request.json -H "Content-Type: application/json" 
  http://localhost:8082/spring-rest/foos/new
curl -d '{"id":9,"name":"baeldung"}' -H 'Content-Type: application/json' 
  http://localhost:8082/spring-rest/foos/new  
curl -d "{\"id\":9,\"name\":\"baeldung\"}" -H "Content-Type: application/json" 
  http://localhost:8082/spring-rest/foos/new
curl -d @request.json -H 'Content-Type: application/json' 
  -X PUT http://localhost:8082/spring-rest/foos/9
curl -X DELETE http://localhost:8082/spring-rest/foos/9
curl -H "Host: com.baeldung" http://example.com/
curl -H "User-Agent:" http://example.com/
curl -d @request.json -H "Content-Type: application/json" 
  -H "Accept: application/json" http://localhost:8082/spring-rest/foos/new      
curl --user baeldung:secretPassword http://example.com/  
curl -H "Authorization: Bearer b1094abc0-54a4-3eab-7213-877142c33fh3" http://example.com/