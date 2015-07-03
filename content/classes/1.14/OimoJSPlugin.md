---
ID_PAGE: 3345
PG_TITLE: OimoJSPlugin
PG_VERSION: 1.14
---

##Members

###updateBodyPosition : (mesh: [AbstractMesh](page.php?p=3269)) =&gt; void


Update the body position according to the mesh position

@param mesh



##Methods

###initialize(iterations) &rarr; void
Initializes the OIMO engine

####Parameters
 | Name | Type | Description
---|---|---|---
optional | iterations | number | Unused parameter
---

###setGravity(gravity) &rarr; void
Sets the gravity

####Parameters
 | Name | Type | Description
---|---|---|---
 | gravity | [Vector3](page.php?p=3327) | The given gravity
---

###registerMesh(mesh, impostor, options) &rarr; any
Registers a mesh

####Parameters
 | Name | Type | Description
---|---|---|---
 | mesh | [AbstractMesh](page.php?p=3269) | The given mesh to register
 | impostor | number | The corresponding impostor
 | options | PhysicsBodyCreationOptions | An object build this way {mass: number, friction: number, restitution: number}
---

###registerMeshesAsCompound(parts, options) &rarr; any
Register meshes as compound

####Parameters
 | Name | Type | Description
---|---|---|---
 | parts | PhysicsCompoundBodyPart[] | The array of object build this way {mesh: [Mesh](page.php?p=3271), impostor: number}
 | options | PhysicsBodyCreationOptions | An object build this way {mass: number, friction: number, restitution: number}
---

###unregisterMesh(mesh) &rarr; void
Removes the mesh from the world

####Parameters
 | Name | Type | Description
---|---|---|---
 | mesh | [AbstractMesh](page.php?p=3269) | The given mesh to remove
---

###applyImpulse(mesh, force, contactPoint) &rarr; void
Applies a force to the mesh at a contact point

####Parameters
 | Name | Type | Description
---|---|---|---
 | mesh | [AbstractMesh](page.php?p=3269) | The given mesh
 | force | [Vector3](page.php?p=3327) | The force to apply to the mesh
 | contactPoint | [Vector3](page.php?p=3327) | The point of the mesh where the force has to be applied
---

###createLink(mesh1, mesh2, pivot1, pivot2, options) &rarr; boolean
Creates a physical link between two meshes

####Parameters
 | Name | Type | Description
---|---|---|---
 | mesh1 | [AbstractMesh](page.php?p=3269) | The first mesh to link
 | mesh2 | [AbstractMesh](page.php?p=3269) | The second mesh to link
 | pivot1 | [Vector3](page.php?p=3327) | The relative position of the first mesh where the link has to be applied
 | pivot2 | [Vector3](page.php?p=3327) | The relative position of the second mesh where the link has to be applied
optional | options | any | @param options
---

###dispose() &rarr; void
Destroys the engine object


###isSupported() &rarr; boolean
Tests if the plugin is usable in the current environement


###runOneStep(time) &rarr; void
Applies the world transformations for the given amount of time

####Parameters
 | Name | Type | Description
---|---|---|---
 | time | number | The given time
---