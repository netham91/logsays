Command: expo start<br/>
logSays: Error: EMFILE: too many open files, watch
    at FSEvent.FSWatcher._handle.onchange <br>
itMeans: Due to Node's asynchronous nature, if you perform a lot of fs.readFile or similar operations in quick succession, you can easily hit your system's maxfiles limit, usually set to 256 on a dev box.   
credits: @Timer , @treygriffith
