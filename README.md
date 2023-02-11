# SwiftUI

# Cheatsheet concepts 

# NavigationLinks 

## Declare a defaultdict object
                
        NavigationLink(destination: DestinationPage(), label: {
                    Text("Sign up")
                })

# TabBar

        Creating tabbar items

        https://www.hackingwithswift.com/quick-start/swiftui/adding-tabview-and-tabitem

# Alert 
        Button()
        .alert("Invalid Login", isPresented: $showingAlert) {
                Button("OK", role: .cancel) { }
            }


        .alert(isPresented:$showingAlert) {
                            Alert(
                                title: Text("Are you sure you want to delete this?"),
                                message: Text("There is no undo"),
                                primaryButton: .destructive(Text("Delete")) {
                                    print("Deleting...")
                                },
                                secondaryButton: .cancel()
                            )
                        }
# Annotated state types 

        https://www.hackingwithswift.com/quick-start/swiftui/whats-the-difference-between-observedobject-state-and-environmentobject
        
# Dynamic lists
        https://www.hackingwithswift.com/quick-start/swiftui/how-to-create-a-list-of-dynamic-items
        
# Writing to Firestore Database
        https://stackoverflow.com/questions/66695215/swiftui-show-the-data-fetched-from-firebase-in-view
