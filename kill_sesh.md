`lsof -wni tcp:3000`     
`lsof -P | grep ‘:3000’ | awk ‘{print $2}’ | xargs kill -9`    
or
`kill -9 $(lsof -i:3000 -t)`
