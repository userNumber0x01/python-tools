# python tools

[!TIP] netcat.py --help
----------------------------------------------------------------------------------
usage: netcat.py [-h] [-c] [-e EXECUTE] [-l] [-p PORT] [-t TARGET] [-u UPLOAD]
NT Net Tool

options:
  -h, --help            show this help message and exit
  -c, --command         command shell
  -e EXECUTE, --execute EXECUTE
                        execute specified command
  -l, --listen          listen
  -p PORT, --port PORT  specified port
  -t TARGET, --target TARGET
                        specified IP
  -u UPLOAD, --upload UPLOAD
                        upload file

Example:
        netcat.py -t 192.168.1.100 -p 5555 -l -c          # command shell
        netcat.py -t 192.168.1.100 -p 5555 -l -u=test.txt # download file
        netcat.py -t 192.168.1.100 -p 5555 -l -e="cat /etc/passwd" #run command
        echo 'ABC' | ./netcat.py -t 192.168.1.108 -p 2048 #send text to server (port=2048)
        netcat.py -t 192.168.1.100 -p 5555 # connect to server
----------------------------------------------------------------------------------
