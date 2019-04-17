import components to be reference

terminology:
exploded view = explosion := a local arrangement of components for use in drafting
NX12 has an "Exploded Views" tab, and the sub-actions refer to an "explosion"
It seems that generating an "explosion" creates an "exploded view", which is NOT the same as a model view.

Arrangements: Current arrangement dictates which components will be hidden/shown ( and perhaps their position?) when the exploded view is created.  Once explosion is created, changing arrangements has no bearing on the exploded view.
switching explosions from the `exploded views` tab associates an explosion with the current model view
^^ once this association has been made, toggling exploded views should be performed from the model view tab, so that drafting associations are not accidentally affected.

best practice for exploded views on drawings:
create model view
create explosion (same as creating exploded view)
associate explosion with model view

Selected (unique) model view, creates a drafting view that defines:
- Unique view oriention
- Component positioning as defined by the associated exploded view