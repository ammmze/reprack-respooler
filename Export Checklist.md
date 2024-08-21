# Export Checklist

Checklist of things to be done to export/publish the project.

* Create new version in OnShape, and update the link in [CAD](./CAD/README.md).
* Export the "Reprack Rewinder Assembled" assembly from OnShape as STEP and place in the [CAD](./CAD/) directory.
* Export all the parts from the "Re-spooler/v2/Export" part studio as STL with the following settings and place them in the [STL](./STL/) directory.
  * Units: Millimeter
  * Resolution: Fine
  * Export unique parts as individual files: Checked
* Remove the "Export - " prefix from the STL files (`rename --subst 'Export - ' '' *.stl`)
