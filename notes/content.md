

# 



- Connecting a OperationId to a Azure End Point

- Upload a File to Azure Function from Connector  (byte)

- Downoad a File through Azure Function using Connector

- ```python
  def processDownload(url,filename=None):
      try:
          r = requests.get(url, allow_redirects=True)
          mimetype="application/octet-stream"
          if filename is not None:
              mimetypeInfo = mimetypes.guess_type(filename)
              if mimetypeInfo[0]!=None:
                  mimetype=mimetypeInfo[0];
          return func.HttpResponse(r.content, mimetype=mimetype)
      except  Exception as ex :
          return func.HttpResponse(
                  json.dumps({"error":str(ex)}),mimetype="application/json",
                  status_code=400)
  
  ```

- 





```python
            return func.HttpResponse(json.dumps({"id":response["Id"]}),mimetype="application/json")
        except  Exception as ex :
                #exc_info = sys.exc_info()
                authInfo={}
                if is_debug==1:
                    authInfo=req.headers["Authorization"]
                #error=''.join(traceback.format_exception(*exc_info))
                return func.HttpResponse(
                json.dumps({"error":str(ex),"at":authInfo}),mimetype="application/json",
                status_code=400
                  
                  
                   return func.HttpResponse(
                json.dumps({"error":"Invalid action"}),
                mimetype="application/json",
                status_code=400
            )
                  
                  
                      if args["parent_folder_id"]!=None:
         data.update({"ParentFolderId":args["parent_folder_id"]})
    if args["source"]!=None:
         data.update({"Source":args["source"]})
```

