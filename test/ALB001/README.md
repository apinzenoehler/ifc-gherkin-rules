| File name                                                         | Expected result | Error log / further info                                                                | Description                                                                              |
|-------------------------------------------------------------------|-----------------|-----------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------|
| pass-alb001-alignment-in-spatial-structure                        | success         |                                                                                         | Benchmark correct file                                                                   |
| fail-alb001-scenario01-no_contained_relation                      | fail            | The instance #23=IfcAlignment('2HT2$vx...FINED.) is not directly contained in IfcSite The instance #426=IfcAlignment('1pJ$fx...FINED.) is not directly contained in IfcSite | There is no IFCRELCONTAINEDINSPATIALSTRUCTURE relation between IFCALIGNMENT and IFCSITE |
| fail-alb001-scenario01-contained_relation_not_directed_to_ifcsite | fail            | The instance #23=IfcAlignment('2HT2$vx...FINED.) is not directly contained in IfcSite The instance #426=IfcAlignment('1pJ$fx...FINED.) is not directly contained in IfcSite| The IFCRELCONTAINEDINSPATIALSTRUCTURE relation links IFCALIGNMENT to IFCBUILDING not IFCSITE    |