
PRACTICE PROJECT
(FS+HTTPS)
let you create notes,read notes,store notes on disk,access everything via HTTPS routes

we are making::
EXAMPLE::
GET/notes
POST/notes:add new note
GET/ notes?id=2 ->get a single notes

fetures :start and HTTP server,PASE POST Request body


//2:jab koi bell bajayga (website kholega)
//req:kaun aaya hai
//res:tum kya jawab doge
//200:all is ok "Haan beta sb sahi hai"
//res.end:jab website khulega tum bol rh ho server is running
//apna ghar ka gate no 3000 oe khole 


const http =require("http");

const server = http.createServer((req, res) => {
  res.writeHead(200, {"Content-Type":"text/plain" });
  res.end("Server is running");
});

server.listen(3000,() => {console.log("Server running on http://localhost:3000");
});
