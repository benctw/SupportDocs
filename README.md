# SupportDocs: DataSource
This branch is where SupportDocs gets its data! You can add, edit, and delete documents here. For usage instructions, check out the `README`'s [usage](https://github.com/aheze/SupportDocs#using-the-github-repository) section in the main branch.

## Data Source JSON URL
<a href="https://raw.githubusercontent.com/benctw/SupportDocs/DataSource/_data/supportdocs_datasource.json">https://raw.githubusercontent.com/benctw/SupportDocs/DataSource/_data/supportdocs_datasource.json</a>

<details markdown="1">
<summary><strong>Show examples</strong></summary>

<hr>

### SwiftUI
```swift
struct SwiftUIExampleView_MinimalCode: View {
    let dataSource = URL(string: "https://raw.githubusercontent.com/benctw/SupportDocs/DataSource/_data/supportdocs_datasource.json")!
    @State var supportDocsPresented = false
    
    var body: some View {
        Button("Present SupportDocs from SwiftUI!") { supportDocsPresented = true }
        .sheet(isPresented: $supportDocsPresented, content: {
            SupportDocsView(dataSource: dataSource, isPresented: $supportDocsPresented)
        })
    }
}
```

### UIKit
```swift
class UIKitExampleController_MinimalCode: UIViewController {
    /**
    Connect this inside the storyboard.
    
    This is just for demo purposes, so it's not connected yet.
    */
    @IBAction func presentButtonPressed(_ sender: Any) {
        let dataSource = URL(string: "https://raw.githubusercontent.com/benctw/SupportDocs/DataSource/_data/supportdocs_datasource.json")!
    
        let supportDocsViewController = SupportDocsViewController(dataSource: dataSource)
        self.present(supportDocsViewController, animated: true, completion: nil)
    }
}
```

<hr>

</details>

## Table of Contents
- [404 Page](https://benctw.github.io/SupportDocs/404) (SupportDocs Integrated File) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/404.md))
- [Apple smoothie](https://benctw.github.io/SupportDocs/Sample-Smoothies/Apple) (smoothies) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-Smoothies/Apple.md))
- [Blueberry smoothie](https://benctw.github.io/SupportDocs/Sample-Smoothies/Blueberry) (smoothies) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-Smoothies/Blueberry.md))
- [Buy blue boba](https://benctw.github.io/SupportDocs/Sample-Boba/BuyBlueBoba) (boba) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-Boba/BuyBlueBoba.md))
- [Buy cream boba](https://benctw.github.io/SupportDocs/Sample-Boba/BuyCreamBoba) (boba) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-Boba/BuyCreamBoba.md))
- [Buy orange boba](https://benctw.github.io/SupportDocs/Sample-Boba/BuyOrangeBoba) (boba) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-Boba/BuyOrangeBoba.md))
- [How to cook pizza](https://benctw.github.io/SupportDocs/Sample-FastFood/HowToCookPizza) (fastFood) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-FastFood/HowToCookPizza.md))
- [How to eat burritos](https://benctw.github.io/SupportDocs/Sample-FastFood/HowToEatBurritos) (fastFood) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-FastFood/HowToEatBurritos.md))
- [How to eat grilled cheese](https://benctw.github.io/SupportDocs/Sample-FastFood/HowToEatGrilledCheese) (fastFood) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-FastFood/HowToEatGrilledCheese.md))
- [How to eat nachos](https://benctw.github.io/SupportDocs/Sample-FastFood/HowToEatNachos) (fastFood) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-FastFood/HowToEatNachos.md))
- [How to eat tacos](https://benctw.github.io/SupportDocs/Sample-FastFood/HowToEatTacos) (fastFood) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-FastFood/HowToEatTacos.md))
- [How to make spaghetti](https://benctw.github.io/SupportDocs/Sample-FastFood/HowToMakeSpaghetti) (fastFood) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-FastFood/HowToMakeSpaghetti.md))
- [How to prepare ramen](https://benctw.github.io/SupportDocs/Sample-FastFood/HowToPrepareRamen) (fastFood) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-FastFood/HowToPrepareRamen.md))
- [Peach smoothie](https://benctw.github.io/SupportDocs/Sample-Smoothies/Peach) (smoothies) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-Smoothies/Peach.md))
- [Plum smoothie](https://benctw.github.io/SupportDocs/Sample-Smoothies/Plum) (smoothies) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-Smoothies/Plum.md))
- [Red berry smoothie](https://benctw.github.io/SupportDocs/Sample-Smoothies/RedBerries) (smoothies) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Sample-Smoothies/RedBerries.md))
- [安裝Python](https://benctw.github.io/SupportDocs/Python/install_python) (python) ([edit](https://github.com/benctw/SupportDocs/edit/DataSource/Python/install_python.md))


## Notes
- Your changes make take up to five minutes to deploy. You can track the deployment progress [here](https://github.com/benctw/SupportDocs/deployments/activity_log?environment=github-pages).
- Do **not** update this file (`README.md`) directly. Your changes will be overriden the next time you push (the GitHub Action will regenerate this file). Instead, update the file in [`_scripts/README.md`](https://github.com/benctw/SupportDocs/edit/DataSource/_scripts/README.md). 