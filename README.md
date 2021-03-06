DTTableViewManager
================

Powerful architecture for UITableView. The idea is to move all datasource methods to separate class, and add many helper methods to manage presentation of your data models.

Warning - setup will sound complex, but once you use it at least once, you will see the benefits. 

## Core features

* Ability to manipulate models in the table view on the fly. No need to worry about datasource methods.
* Clean controller code
* Table view cells can be created from code, or from IB.
* You can make your controller a subclass of DTTableViewManager, or you can make it a property on your controller and subclass from whatever you need
* Any datasource/delegate method can be overridden in your controller

## Requirements

* iOS 5.0
* ARC
        
## Installation

Simplest option is to use [CocoaPods](http://www.cocoapods.org):

	pod 'DTTableViewManager'
	
## Example 

Example project is available in Example folder. 

## Documentation

You can view documentation [online](http://denheadless.github.com/DTTableViewManager/) or you can install it locally using following atom link: [http://denheadless.github.com/DTTableViewManager/DTTableViewManager.atom](http://denheadless.github.com/DTTableViewManager/DTTableViewManager.atom).

## Discussion

This approach intends to clean your view controller from massive amounts of repeatable datasource code. It helps to think about table view models instead of table view cells. Table view cells should be responsive for displaying their content, and controller should only be responsive for displaying models, not cells. 

[Changelog](https://github.com/DenHeadless/DTTableViewManager/wiki/Changelog)
		
## Thanks

Special thanks to Alexey Belkevich (https://github.com/belkevich) for providing initial implementation of CellFactory.
Thanks to @lukeredpath for awesome [GCDSingleton macro](https://gist.github.com/1057420).