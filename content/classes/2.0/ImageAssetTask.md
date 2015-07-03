---
ID_PAGE: 5869
PG_TITLE: ImageAssetTask
PG_VERSION: 2.0
---

Load task on the given image
##new [ImageAssetTask](page.php?p=5869)(name, url)


The [ImageAssetTask](page.php?p=5869)


####Parameters
 | Name | Type | Description
---|---|---|---
 | name | string | The name
 | url | string | The url to this image
---

##Members

###name : string



The name


###url : string



The url to this image


###onSuccess : (task: IAssetTask) =&gt; void



Function call when the mesh is load successfully


###onError : (task: IAssetTask) =&gt; void



Function call when the mesh isn't load successfully


###isCompleted : boolean



True if is completed, false otherwise.


###image : HTMLImageElement



The image







##Methods

###run(scene, onSuccess, onError) &rarr; void

####Parameters
 | Name | Type | Description
---|---|---|---
 | scene | [Scene](page.php?p=5725) | the scene where the image is.
 | onSuccess | () =&gt; void | Function call when the mesh is load successfully
 | onError | () =&gt; void | Function call when the mesh isn't load successfully
---