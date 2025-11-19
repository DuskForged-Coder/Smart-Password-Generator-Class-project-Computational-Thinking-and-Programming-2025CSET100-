 ┌────────────────────────────────┐
 │         START APPLICATION      │
 └───────────────┬────────────────┘
                 │
                 ▼
     ┌───────────────────────────┐
     │ Initialize CTk Window     │
     │ • Dark theme              │
     │ • Set fonts               │
     │ • Window size             │
     └──────────────┬────────────┘
                    │
                    ▼
       ┌─────────────────────────┐
       │ Build Main UI           │
       │ • Title                 │
       │ • Length slider         │
       │ • Checkboxes (options)  │
       │ • Output box            │
       │ • Buttons               │
       │ • History button        │
       └─────────────┬───────────┘
                     │
                     ▼
        ┌──────────────────────────┐
        │ User Clicks "Generate"   │
        └──────────────┬───────────┘
                       │
                       ▼
      ┌─────────────────────────────────┐
      │ generate_password()             │
      │ • Build character pool          │
      │ • Apply options (upper, lower)  │
      │ • Remove ambiguous if selected  │
      │ • Randomly choose characters    │
      │ • Return final password         │
      └─────────────────┬──────────────┘
                        │
                        ▼
         ┌──────────────────────────┐
         │ Display Password in UI   │
         └─────────────┬────────────┘
                       │
                       ├─────────────► User copies password
                       │               (clipboard function)
                       │
                       ▼
         ┌──────────────────────────┐
         │ User Clicks "Save"       │
         └──────────────┬───────────┘
                        │
                        ▼
       ┌─────────────────────────────────┐
       │ Save Popup Window               │
       │ User enters label               │
       │ save_password() writes to CSV   │
       └───────────────────┬────────────┘
                           │
                           ▼
         ┌─────────────────────────────┐
         │ CSV Updated (timestamp +    │
         │ label + password)           │
         └─────────────────┬──────────┘
                           │
                           ▼
            ┌──────────────────────────┐
            │ User Clicks "View History"  
            └──────────────┬───────────┘
                           │
                           ▼
        ┌───────────────────────────────────┐
        │ Build History Window (CTkToplevel)│
        │ Load CSV                          │
        │ Show in ttk.Treeview table        │
        │ "Export CSV" button               │
        └────────────────────┬──────────────┘
                             │
                             ▼
            ┌──────────────────────────────┐
            │ User chooses export location │
            │ via filedialog               │
            │ CSV copied using shutil      │
            └──────────────────────────────┘
                             │
                             ▼
                  ┌───────────────────┐
                  │       END         │
                  └───────────────────┘
