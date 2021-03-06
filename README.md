## ITWLoadingPanel
ITWLoadingPanel is a class for adding a download info panel, made at [Intotheweb](http://intotheweb.be/)

![Screenshot](https://github.com/brunow/ITWLoadingPanel/raw/master/Screenshot.png)

## Compatibility

ITWLoadingPanel work with both iPad and iPhone in any orientation.

## Installation

Copy ITWLoadingPanel or install it with **cocoapods**

	dependency 'ITWLoadingPanel', '~> 1.0.1'

## How to use it

Show it:

	[ITWLoadingPanel showPanelInView:self.view title:@"Title" cancelTitle:@"Cancel"];

Hide it:

	[ITWLoadingPanel  hidePanel];

## How to customize it

Subclass ITWLoadingPanel and do customization inside awakeFromNib:

	- (void)awakeFromNib {
 	   [super awakeFromNib];
    
	    self.backgroundColor = [UIColor redColor];
	    [self.cancelBtn setBackgroundImage:image forState:state];
	    self.cancelLabel.textColor = [UIColor yellowColor];
	    self.titleLabel.textColor = [UIColor blackColor];
	}

# App using ITWLoadingPanel

If you use ITWLoadingPanel I'll be happy to add your app name here.

[LiègeExpo2017](http://itunes.apple.com/fr/app/liege-expo-2017/id505451794?mt=8)

## ARC
ITWLoadingPanel is fully compatible out of box with both ARC and non-ARC project.