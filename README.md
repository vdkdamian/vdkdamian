# 👋 Hello, I'm Damian

```swift
struct Developer {
    let firstname = "Damian"
    let lastname = "Van de Kauter"
    var fullname: String { PersonNameComponents(developer: self).fullname }
    
    let role: String = "Developer"
    let language: String = "Swift"
    let tools: [String] = ["SwiftUI", "SwiftData", "Swift Macros", "Xcode"]
    
    let location: String = "Belgium 🇧🇪"
}

extension Developer: CustomStringConvertible {
    var description: String {
        "\(fullname), \(role) working in \(language) – based in \(location)"
    }
}

extension PersonNameComponents {
    
    init(developer: Developer) {
        self.init()
        self.givenName = developer.firstname
        self.familyName = developer.lastname
    }
    
    var fullname: String {
        Self.nameFormatter.string(from: self)
    }
    
    private static let nameFormatter = PersonNameComponentsFormatter()
}
```

🚀 I build performant, elegant apps using Swift and SwiftUI.

“Readable code is good. Fast and correct code is better. I try to do all three.”

<h4>Social media</h4>

[![Linkedin: damianvandekauter](https://img.shields.io/badge/-DamianVandeKauter-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/vdkdamian)](https://www.linkedin.com/in/vdkdamian)
