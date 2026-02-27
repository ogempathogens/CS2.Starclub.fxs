# IDA Sigs


## Repository made for finding signatures in random games.


# Counter-Strike 2
| Name | Binary | Function | STR | Instruction |
| :---         |     :---:      |     :---:     |     :---:     |     :---:     |
| CalculateWorldSpaceBones   | client.dll     | sub_180A0ADF0    | Bone merge bones from parent were invalid: parent model '%s': our model '%s' <br> Flags: %X (%X)    | xref -> go to the top -> first instruction        |
| RunCommand     | client.dll       | sub_1809C9F30      | runcommand:%04d      | X        |
| EquipItemInLoadout     | client.dll       | sub_1807BB960      | \nLOADOUT ACTION BATCH #%i\n      | xref -> go to the top -> first instruction        |
| UpdateSubClass     | client.dll       | sub_180A74DB0      | OnSubclassIDChanged      | X        |

# FiveM 
| Name | Binary | Function | STR | Instruction |
| :---         |     :---:      |     :---:     |     :---:     |     :---:     |
| CoreGetComponentRegistry   | CoreRT.dll     | X    | X    | Exports -> search for 'CoreGetComponentRegistry' -> make sig        |
| fx::ResourceManager::getCurrent     | citizen-resources-core.dll       | X      | X      | Exports -> search for 'fx::ResourceManager::GetCurrent(bool)' -> make sig       |

// Provided by empathogens 
