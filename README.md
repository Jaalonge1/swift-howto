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
