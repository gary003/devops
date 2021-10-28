1. Basic call of curl (GET). returns a todo from json placeholder(fake API)
-- curl https://jsonplaceholder.typicode.com/todos/1

2. -i . includes the headers with the response
-- curl -i https://jsonplaceholder.typicode.com/todos/1

3. If we only want the headers
-- curl -i https://jsonplaceholder.typicode.com/todos/1

4. Save the result in a file
-- curl -o fileRes.txt https://jsonplaceholder.typicode.com/todos/1

5. Download a file with curl.
!! the file needs to exist on the remote server (you can't download one todo) !!
It also work with images.
-- curl -O https://jsonplaceholder.typicode.com/todos

6. Put a limit on the data transfert.
-- curl -O --limit-rate 200B https://jsonplaceholder.typicode.com/todos

7. Make a post request
-- curl -X POST --data "userId=1,title='insert post',completed=false" https://jsonplaceholder.typicode.com/todos

8. Make a put request. (-d is small for --data)
-- curl -X PUT -d "title='modified post'" https://jsonplaceholder.typicode.com/todos/12

9. Make a put request.
-- curl -X DELETE https://jsonplaceholder.typicode.com/todos/12

10. Authentification for request
-- curl -u <username>:<password> https://jsonplaceholder.typicode.com/todos/12

10. Authentificate with a token.
-- curl -H "Authorization: OAuth <ACCESS_TOKEN>" http://www.example.com

11. Follow a redirection.
-- curl -L https://google.com

12. Download a ftp file
-- curl -u <username>@<ftpAccount>:<password> -T nameOfFileToDDL url

