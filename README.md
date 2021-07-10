# swift-howto
Repo for myself to learn GitHub &amp; all about SwiftUI.

---
**IMAGES** https://developer.apple.com/documentation/swiftui/image
---
        Image("Landscape_4")
          .resizable()
          .aspectRatio(contentMode: .fit)
        Text("Water wheel")

---
**SHAPES** https://www.hackingwithswift.com/quick-start/swiftui/swiftuis-built-in-shapes
---
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
**CONTROL FLOW**
---

---
**FOR IN LOOPS** https://docs.swift.org/swift-book/LanguageGuide/ControlFlow.html
---
You use the for-in loop to iterate over a sequence, such as items in an array, ranges of numbers, or characters in a string.

        This example uses a for-in loop to iterate over the items in an array:

        let names = ["Anna", "Alex", "Brian", "Jack"]
        for name in names {
            print("Hello, \(name)!")
        }
        // Hello, Anna!
        // Hello, Alex!
        // Hello, Brian!
        // Hello, Jack!
       
* You can also iterate over a dictionary to access its key-value pairs. Each item in the dictionary is returned as a (key, value) tuple when the dictionary is iterated

In some situations, you might not want to use closed ranges, which include both endpoints. Consider drawing the tick marks for every minute on a watch face. You want to draw 60 tick marks, starting with the 0 minute. Use the half-open range operator (..<) to include the lower bound but not the upper bound. For more about ranges, see Range Operators.

        let minutes = 60
        for tickMark in 0..<minutes {
            // render the tick mark each minute (60 times)
        }
        
Some users might want fewer tick marks in their UI. They could prefer one mark every 5 minutes instead. Use the stride(from:to:by:) function to skip the unwanted marks.

        let minuteInterval = 5
        for tickMark in stride(from: 0, to: minutes, by: minuteInterval) {
            // render the tick mark every 5 minutes (0, 5, 10, 15 ... 45, 50, 55)
        }
Closed ranges are also available, by using stride(from:through:by:) instead:

        let hours = 12
        let hourInterval = 3
        for tickMark in stride(from: 3, through: hours, by: hourInterval) {
            // render the tick mark every 3 hours (3, 6, 9, 12)
        }
---
