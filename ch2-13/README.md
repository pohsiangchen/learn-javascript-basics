# Conceptual Aside: Single Threaded, Synchronous Execution


### Single Threaded: one command at a time
* 同一個時段內只會有一段代碼在執行
* 單就 Javascript engine來說，它是 single thread 方式運作，然而在整個瀏覽器中，同時間不只處理 Javascript 的內容，可以是 multi-threaded 


### Synchronous: one at a time
* 一次只能完成一件事，待完成後再處理下一件   
     
    
    
## Javascript 以 Single threaded, synchronous execution 方式運行

```javascript
    1 thread ->   |<---A---->||<----B---------->||<------C----->|
```

PS ref: http://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean
