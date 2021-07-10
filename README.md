# swift-howto
Repo for myself to learn GitHub &amp; all about SwiftUI.

---
**IMAGES** https://developer.apple.com/documentation/swiftui/image

        Image("Landscape_4")
          .resizable()
          .aspectRatio(contentMode: .fit)
        Text("Water wheel")

---
**SHAPES** https://www.hackingwithswift.com/quick-start/swiftui/swiftuis-built-in-shapes
   
        Rectangle()
            .fill(Color.black)
            .frame(width: 200, height: 200)

        RoundedRectangle(cornerRadius: 25, style: .continuous)
            .fill(Color.red)
            .frame(width: 200, height: 200)

        Capsule()
            .fill(Color.green)
            .frame(width: 100, height: 50)

        Ellipse()
            .fill(Color.blue)
            .frame(width: 100, height: 50)

        Circle()
            .fill(Color.white)
            .frame(width: 100, height: 50)
            
* tip : if you want to give a Rectange rounded corners, use RoundedRectangle() not Rectangle()! 
        * https://stackoverflow.com/questions/62970198/trying-to-give-a-border-a-corner-radius-in-swiftui
---

