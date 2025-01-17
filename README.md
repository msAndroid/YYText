YYText <a href="#中文介绍">中文介绍</a>
==============
[![License MIT](https://img.shields.io/badge/license-MIT-green.svg?style=flat)](https://raw.githubusercontent.com/ibireme/YYText/master/LICENSE)&nbsp;
[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)&nbsp;
[![Cocoapods](http://img.shields.io/cocoapods/v/YYText.svg?style=flat)](http://cocoapods.org/?q= YYText)&nbsp;
[![Cocoapods](http://img.shields.io/cocoapods/p/YYText.svg?style=flat)](http://cocoapods.org/?q= YYText)&nbsp;
[![Support](https://img.shields.io/badge/support-iOS%206%2B%20-blue.svg?style=flat)](https://www.apple.com/nl/ios/)&nbsp;
[![Build Status](https://travis-ci.org/ibireme/YYText.svg?branch=master)](https://travis-ci.org/ibireme/YYText)

Powerful text framework for iOS to display and edit rich text.<br/>
(It's a component of [YYKit](https://github.com/ibireme/YYKit))


Features
==============

- UILabel and UITextView API compatible
- High performance synchronous text layout and rendering
- Extended CoreText attributes with more text effects
- Text attachments with UIImage, UIView and CALayer
- Custom highlight text range to allow user interact with
- Text parser support (built in markdown/emoticon parser)
- Text container path and exclusion paths support
- Vertical form layout support
- Image and attributed text copy/paste support
- Attributed text placeholder support
- Custom keyboard view support
- Undo and redo control
- Attributed text archiver and unarchiver support
- Multi-language and VoiceOver support
- Fully documented

Architecture
==============
YYText vs TextKit

<img src="https://raw.github.com/ibireme/YYText/master/Attributes/architecture.png" width="400">


Text Attributes
==============

### YYText supported attributes
<table>
  <thead>
    <tr>
      <th>Demo</th>
      <th>Attribute Name</th>
      <th>Class</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextBackedString.png" width="200"></td>
      <td>TextBackedString</td>
      <td>YYTextBackedString</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextBinding.gif" width="200"></td>
      <td>TextBinding</td>
      <td>YYTextBinding</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextShadow.png" width="200"></td>
      <td>TextShadow</td>
      <td>YYTextShadow</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextShadow.png" width="200"></td>
      <td>TextInnerShadow</td>
      <td>YYTextShadow</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Underline.png" width="200"></td>
      <td>TextUnderline</td>
      <td>YYTextDecoration</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Strikethrough.png" width="200"></td>
      <td>TextStrickthrough</td>
      <td>YYTextDecoration</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextBorder.png" width="200"></td>
      <td>TextBorder</td>
      <td>YYTextBorder</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextBackgroundBorder.png" width="200"></td>
      <td>TextBackgroundBorder</td>
      <td>YYTextBorder</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextBlockBorder.png" width="200"></td>
      <td>TextBlockBorder</td>
      <td>YYTextBorder</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextAttachment.gif" width="200"></td>
      <td>TextAttachment</td>
      <td>YYTextAttachment</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextHighlight.gif" width="200"></td>
      <td>TextHighlight</td>
      <td>YYTextHighlight</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Obliqueness.png" width="200"></td>
      <td>TextGlyphTransform</td>
      <td> NSValue(CGAffineTransform)</td>
    </tr>
  </tbody>
</table>

###CoreText attributes which is supported by YYText
<table>
  <thead>
    <tr>
      <th>Demo</th>
      <th>Attribute Name</th>
      <th>Class</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Font.png" width="200"></td>
      <td> Font </td>
      <td>UIFont(CTFontRef)</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Kern.png" width="200"></td>
      <td> Kern </td>
      <td>NSNumber</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Stroke.png" width="200"></td>
      <td> StrokeWidth </td>
      <td> NSNumber </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/StrokeColor.png" width="200"></td>
      <td> StrokeColor </td>
      <td> CGColorRef </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Shadow.png" width="200"></td>
      <td> Shadow </td>
      <td> NSShadow </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Ligature.png" width="200"></td>
      <td> Ligature </td>
      <td> NSNumber </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/VerticalForms.png" width="200"></td>
      <td> VerticalGlyphForm </td>
      <td> NSNumber(BOOL) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/WriteDirection.png" width="200"></td>
      <td> WritingDirection </td>
      <td> NSArray(NSNumber) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/RunDelegate.png" width="200"></td>
      <td> RunDelegate </td>
      <td> CTRunDelegateRef </td>
    </tr>
    
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/Alignment.png" width="200"></td>
      <td> TextAlignment </td>
      <td> NSParagraphStyle <br/>(NSTextAlignment) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/LineBreakMode.png" width="200"></td>
      <td> LineBreakMode </td>
      <td> NSParagraphStyle <br/>(NSLineBreakMode) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/LineSpacing.png" width="200"></td>
      <td> LineSpacing </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/ParagraphSpacing.png" width="200"></td>
      <td> ParagraphSpacing <br/> ParagraphSpacingBefore </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/FirstLineHeadIndent.png" width="200"></td>
      <td> FirstLineHeadIndent </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/HeadIndent.png" width="200"></td>
      <td> HeadIndent </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/TailIndent.png" width="200"></td>
      <td> TailIndent </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/MinimumLineHeight.png" width="200"></td>
      <td> MinimumLineHeight </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/MaximumLineHeight.png" width="200"></td>
      <td> MaximumLineHeight </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/LineHeightMultiple.png" width="200"></td>
      <td> LineHeightMultiple </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/BaseWritingDirection.png" width="200"></td>
      <td> BaseWritingDirection </td>
      <td> NSParagraphStyle <br/>(NSWritingDirection) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/Tab.png" width="200"></td>
      <td> DefaultTabInterval <br/> TabStops </td>
      <td> NSParagraphStyle <br/>CGFloat/NSArray(NSTextTab)</td>
    </tr>
  </tbody>
</table>


Usage
==============

### Basic
    // YYLabel (similar to UILabel)
    YYLabel *label = [YYLabel new];
    label.frame = ...
    label.font = ...
    label.textColor = ...
    label.textAlignment = ...
    label.lineBreakMode = ...
    label.numberOfLines = ...
    label.text = ...
    
    // YYTextView (similar to UITextView)
    YYTextView *textView = [YYTextView new];
    textView.frame = ...
    textView.font = ...
    textView.textColor = ...
    textView.dataDetectorTypes = ...
    textView.placeHolderText = ...
    textView.placeHolderTextColor = ...
    textView.delegate = ...
    

### Attributed text
    
    // 1. Create an attributed string.
    NSMutableAttributedString *text = [[NSMutableAttributedString alloc] initWithString:@"Some Text, blabla..."];
    
    // 2. Set attributes to text, you can use almost all CoreText attributes.
    text.yy_font = [UIFont boldSystemFontOfSize:30];
    text.yy_color = [UIColor blueColor];
    [text yy_setColor:[UIColor redColor] range:NSmakeRange(0, 4)];
    text.yy_lineSpacing = 10;
    
    // 3. Set to YYLabel or YYTextView.
    YYLabel *label = [YYLabel new];
    label.frame = ...
    label.attributedString = text;
    
    YYTextView *textView = [YYTextiew new];
    textView.frame = ...
    textView.attributedString = text;
    
### Text highlight
    
    // 1. Create a 'highlight' attribute for text.
    YYTextBorder *border = [YYTextBorder borderWithFillColor:[UIColor grayColor] cornerRadius:3];
        
    YYTextHighlight *highlight = [YYTextHighlight new];
    [highlight setColor:[UIColor whiteColor]];
    [highlight setBackgroundBorder:highlightBorder];
    highlight.tapAction = ^(UIView *containerView, NSAttributedString *text, NSRange range, CGRect rect) {
      NSLog(@"tap text range:..."); 
      // you can also set the action handler to YYLabel or YYTextView.
    };
    
    // 2. Add 'highlight' attribute to a range of text.
    [attributedText yy_setTextHighlight:highlight range:highlightRange];
    
    // 3. Set text to label or text view.
    YYLabel *label = ...
    label.attributedText = attributedText
    
    YYTextView *textView = ...
    textView.attributedText = ...
    
    // 4. Receive user interactive action.
    label.highlightTapAction = ^(UIView *containerView, NSAttributedString *text, NSRange range, CGRect rect) {
        NSLog(@"tap text range:...");
    };
    label.highlightLongPressAction = ^(UIView *containerView, NSAttributedString *text, NSRange range, CGRect rect) {
        NSLog(@"long press text range:...");
    };
    
    @UITextViewDelegate
    - (void)textView:(YYTextView *)textView didTapHighlight:(YYTextHighlight *)highlight inRange:(NSRange)characterRange rect:(CGRect)rect {
        NSLog(@"tap text range:...");
    }
    - (void)textView:(YYTextView *)textView didLongPoressHighlight:(YYTextHighlight *)highlight inRange:(NSRange)characterRange rect:(CGRect)rect {
        NSLog(@"long press text range:...");
    }


### Text attachments

	NSMutableAttributedString *text = [NSMutableAttributedString new];
	UIFont *font = [UIFont systemFontOfSize:16];
	NSMutableAttributedString *attachment = nil;
	
	// UIImage attachment
	UIImage *image = [UIImage imageNamed:@"dribbble64_imageio"];
	attachment = [NSMutableAttributedString yy_attachmentStringWithContent:image contentMode:UIViewContentModeCenter attachmentSize:image.size alignToFont:font alignment:YYTextVerticalAlignmentCenter];
	[text appendAttributedString: attachment];
	
	// UIView attachment
	UISwitch *switcher = [UISwitch new];
    [switcher sizeToFit];
	attachment = [NSMutableAttributedString yy_attachmentStringWithContent: switcher contentMode:UIViewContentModeBottom attachmentSize:switcher.size alignToFont:font alignment:YYTextVerticalAlignmentCenter];
	[text appendAttributedString: attachment];
	
	// CALayer attachment
	CASharpLayer *layer = [CASharpLayer layer];
	layer.path = ...
	attachment = [NSMutableAttributedString yy_attachmentStringWithContent: layer contentMode:UIViewContentModeBottom attachmentSize:switcher.size alignToFont:font alignment:YYTextVerticalAlignmentCenter];
	[text appendAttributedString: attachment];
	
	
### Asynchronous layout and rendering
    
    // If you have performance issues,
    // you may enable the asynchronous display mode.
    YYLabel *label = ...
    label.displaysAsynchronously = YES;
    
    // If you want to get the highest performance, you should do 
    // text layout with `YYTextLayout` class in background thread.
    YYLabel *label = [YYLabel new];
    label.displaysAsynchronously = YES;
    label.ignoreCommonProperties = YES;
    
    dispatch_async(dispatch_get_global_queue(DISPATCH_QUEUE_PRIORITY_DEFAULT, 0), ^{
        // Create attributed string.
        NSMutableAttributedString *text = [[NSMutableAttributedString alloc] initWithString:@"Some Text"];
        text.yy_font = [UIFont systemFontOfSize:16];
        text.yy_color = [UIColor grayColor];
        [text yy_setColor:[UIColor redColor] range:NSMakeRange(0, 4)];
 
        // Create text container
        YYTextContainer *container = [YYTextContainer new];
        container.size = CGSizeMake(100, CGFLOAT_MAX);
        container.maximumNumberOfRows = 0;
        
        // Generate a text layout.
        YYTextLayout *layout = [YYTextLayout layoutWithContainer:container text:text];
        
        dispatch_async(dispatch_get_main_queue(), ^{
            label.size = layout.textBoundingSize;
            label.textLayout = layout;
        });
    });

### Text container control

	YYLabel *label = ...
	label.textContainerPath = [UIBezierPath bezierPathWith...];
	label.exclusionPaths = 	@[[UIBezierPath bezierPathWith...];,...];
	label.textContainerInset = UIEdgeInserMake(...);
	label.verticalForm = YES/NO;
    
    YYTextView *textView = ...
	textView.exclusionPaths = 	@[[UIBezierPath bezierPathWith...];,...];
	textView.textContainerInset = UIEdgeInserMake(...);
	textView.verticalForm = YES/NO;
    
### Text parser
	// 1. Create a text parser
	
    YYTextSimpleEmoticonParser *parser = [YYTextSimpleEmoticonParser new];
    NSMutableDictionary *mapper = [NSMutableDictionary new];
    mapper[@":smile:"] = [UIImage imageNamed:@"smile.png"];
    mapper[@":cool:"] = [UIImage imageNamed:@"cool.png"];
    mapper[@":cry:"] = [UIImage imageNamed:@"cry.png"];
    mapper[@":wink:"] = [UIImage imageNamed:@"wink.png"];
    parser.emoticonMapper = mapper;
	
	YYTextSimpleMarkdownParser *parser = [YYTextSimpleMarkdownParser new];
    [parser setColorWithDarkTheme];
    
    MyCustomParser *parser = ... // custom parser
    
    // 2. Attach parser to label or text view
    YYLabel *label = ...
    label.textParser = parser;
    
    YYTextView *textView = ...
    textView.textParser = parser;


### More examples
See `Demo/YYTextDemo.xcodeproj` for more examples:

<img src="https://raw.github.com/ibireme/YYText/master/Demo/DemoSnapshot/text_path.gif" width="320">
<img src="https://raw.github.com/ibireme/YYText/master/Demo/DemoSnapshot/text_markdown.gif" width="320">
<br/> <br/>
<img src="https://raw.github.com/ibireme/YYText/master/Demo/DemoSnapshot/text_vertical.gif" width="320">
<img src="https://raw.github.com/ibireme/YYText/master/Demo/DemoSnapshot/text_paste.gif" width="320">


Installation
==============

### Cocoapods

1. Add `pod "YYText"` to your Podfile.
2. Run `pod install` or `pod update`.
3. Import \<YYText/YYText.h\>


### Carthage

1. Add `github "ibireme/YYText"` to your Cartfile.
2. Run `carthage update --platform ios` and add the framework to your project.
3. Import \<YYText/YYText.h\>


### Manually

1. Download all the files in the `YYText` subdirectory.
2. Add the source files to your Xcode project.
3. Link with required frameworks:
    * UIKit
    * CoreFoundation
    * CoreText
    * QuartzCore
    * Accelerate
    * MobileCoreServices
4. Add [YYImage](https://github.com/ibireme/YYImage) if you want to support animated image copy and paste.
5. Import `YYText.h`.

Documentation
==============
Full API documentation is available on [CocoaDocs](http://cocoadocs.org/docsets/YYText/).<br/>
You can also install documentation locally using [appledoc](https://github.com/tomaz/appledoc).

Requirements
==============
This library requires a deployment target of iOS 6.0 or greater.


License
==============
YYText is released under the MIT license. See LICENSE file for details.


<br/><br/>
---
中文介绍
==============
功能强大的 iOS 富文本编辑与显示框架。<br/>
(该项目是 [YYKit](https://github.com/ibireme/YYKit) 组件之一)

特性
==============
- API 兼容 UILabel 和 UITextView
- 支持高性能的异步排版和渲染
- 扩展了 CoreText 的属性以支持更多文字效果
- 支持 UIImage、UIView、CALayer 作为图文混排元素
- 支持添加自定义样式的、可点击的文本高亮范围
- 支持自定义文本解析 (内置简单的 Markdown/表情解析)
- 支持文本容器路径、内部留空路径的控制
- 支持文字竖排版，可用于编辑和显示中日韩文本
- 支持图片和富文本的复制粘贴
- 文本编辑时，支持富文本占位符
- 支持自定义键盘视图
- 撤销和重做次数的控制
- 富文本的序列化与反序列化支持
- 支持多语言，支持 VoiceOver
- 全部代码都有文档注释



架构
==============
YYText 和 TextKit 架构对比

<img src="https://raw.github.com/ibireme/YYText/master/Attributes/architecture.png" width="400">


文本属性
==============

### YYText 原生支持的属性
<table>
  <thead>
    <tr>
      <th>Demo</th>
      <th>Attribute Name</th>
      <th>Class</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextBackedString.png" width="200"></td>
      <td>TextBackedString</td>
      <td>YYTextBackedString</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextBinding.gif" width="200"></td>
      <td>TextBinding</td>
      <td>YYTextBinding</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextShadow.png" width="200"></td>
      <td>TextShadow</td>
      <td>YYTextShadow</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextShadow.png" width="200"></td>
      <td>TextInnerShadow</td>
      <td>YYTextShadow</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Underline.png" width="200"></td>
      <td>TextUnderline</td>
      <td>YYTextDecoration</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Strikethrough.png" width="200"></td>
      <td>TextStrickthrough</td>
      <td>YYTextDecoration</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextBorder.png" width="200"></td>
      <td>TextBorder</td>
      <td>YYTextBorder</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextBackgroundBorder.png" width="200"></td>
      <td>TextBackgroundBorder</td>
      <td>YYTextBorder</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextBlockBorder.png" width="200"></td>
      <td>TextBlockBorder</td>
      <td>YYTextBorder</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextAttachment.gif" width="200"></td>
      <td>TextAttachment</td>
      <td>YYTextAttachment</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/YYText Extended/YYTextHighlight.gif" width="200"></td>
      <td>TextHighlight</td>
      <td>YYTextHighlight</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Obliqueness.png" width="200"></td>
      <td>TextGlyphTransform</td>
      <td> NSValue(CGAffineTransform)</td>
    </tr>
  </tbody>
</table>

###YYText 支持的 CoreText 属性
<table>
  <thead>
    <tr>
      <th>Demo</th>
      <th>Attribute Name</th>
      <th>Class</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Font.png" width="200"></td>
      <td> Font </td>
      <td>UIFont(CTFontRef)</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Kern.png" width="200"></td>
      <td> Kern </td>
      <td>NSNumber</td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Stroke.png" width="200"></td>
      <td> StrokeWidth </td>
      <td> NSNumber </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/StrokeColor.png" width="200"></td>
      <td> StrokeColor </td>
      <td> CGColorRef </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Shadow.png" width="200"></td>
      <td> Shadow </td>
      <td> NSShadow </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Ligature.png" width="200"></td>
      <td> Ligature </td>
      <td> NSNumber </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/VerticalForms.png" width="200"></td>
      <td> VerticalGlyphForm </td>
      <td> NSNumber(BOOL) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/WriteDirection.png" width="200"></td>
      <td> WritingDirection </td>
      <td> NSArray(NSNumber) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/RunDelegate.png" width="200"></td>
      <td> RunDelegate </td>
      <td> CTRunDelegateRef </td>
    </tr>
    
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/Alignment.png" width="200"></td>
      <td> TextAlignment </td>
      <td> NSParagraphStyle <br/>(NSTextAlignment) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/LineBreakMode.png" width="200"></td>
      <td> LineBreakMode </td>
      <td> NSParagraphStyle <br/>(NSLineBreakMode) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/LineSpacing.png" width="200"></td>
      <td> LineSpacing </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/ParagraphSpacing.png" width="200"></td>
      <td> ParagraphSpacing <br/> ParagraphSpacingBefore </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/FirstLineHeadIndent.png" width="200"></td>
      <td> FirstLineHeadIndent </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/HeadIndent.png" width="200"></td>
      <td> HeadIndent </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/TailIndent.png" width="200"></td>
      <td> TailIndent </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/MinimumLineHeight.png" width="200"></td>
      <td> MinimumLineHeight </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/MaximumLineHeight.png" width="200"></td>
      <td> MaximumLineHeight </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/LineHeightMultiple.png" width="200"></td>
      <td> LineHeightMultiple </td>
      <td> NSParagraphStyle <br/>(CGFloat) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/BaseWritingDirection.png" width="200"></td>
      <td> BaseWritingDirection </td>
      <td> NSParagraphStyle <br/>(NSWritingDirection) </td>
    </tr>
    <tr>
      <td><img src="https://raw.github.com/ibireme/YYText/master/Attributes/CoreText and TextKit/Paragraph/Tab.png" width="200"></td>
      <td> DefaultTabInterval <br/> TabStops </td>
      <td> NSParagraphStyle <br/>CGFloat/NSArray(NSTextTab)</td>
    </tr>
  </tbody>
</table>


用法
==============

### 基本用法
    // YYLabel (和 UILabel 用法一致)
    YYLabel *label = [YYLabel new];
    label.frame = ...
    label.font = ...
    label.textColor = ...
    label.textAlignment = ...
    label.lineBreakMode = ...
    label.numberOfLines = ...
    label.text = ...
    
    // YYTextView (和 UITextView 用法一致)
    YYTextView *textView = [YYTextView new];
    textView.frame = ...
    textView.font = ...
    textView.textColor = ...
    textView.dataDetectorTypes = ...
    textView.placeHolderText = ...
    textView.placeHolderTextColor = ...
    textView.delegate = ...
    

### 属性文本
    
    // 1. 创建一个属性文本
    NSMutableAttributedString *text = [[NSMutableAttributedString alloc] initWithString:@"Some Text, blabla..."];
    
    // 2. 为文本设置属性
    text.yy_font = [UIFont boldSystemFontOfSize:30];
    text.yy_color = [UIColor blueColor];
    [text yy_setColor:[UIColor redColor] range:NSmakeRange(0, 4)];
    text.yy_lineSpacing = 10;
    
    // 3. 赋值到 YYLabel 或 YYTextView
    YYLabel *label = [YYLabel new];
    label.frame = ...
    label.attributedString = text;
    
    YYTextView *textView = [YYTextiew new];
    textView.frame = ...
    textView.attributedString = text;
    
### 文本高亮
    
    // 1. 创建一个"高亮"属性，当用户点击了高亮区域的文本时，"高亮"属性会替换掉原本的属性
    YYTextBorder *border = [YYTextBorder borderWithFillColor:[UIColor grayColor] cornerRadius:3];
        
    YYTextHighlight *highlight = [YYTextHighlight new];
    [highlight setColor:[UIColor whiteColor]];
    [highlight setBackgroundBorder:highlightBorder];
    highlight.tapAction = ^(UIView *containerView, NSAttributedString *text, NSRange range, CGRect rect) {
      NSLog(@"tap text range:..."); 
      // 你也可以把事件回调放到 YYLabel 和 YYTextView 来处理。
    };
    
    // 2. 把"高亮"属性设置到某个文本范围
    [attributedText yy_setTextHighlight:highlight range:highlightRange];
    
    // 3. 把属性文本设置到 YYLabel 或 YYTextView
    YYLabel *label = ...
    label.attributedText = attributedText
    
    YYTextView *textView = ...
    textView.attributedText = ...
    
    // 4. 接受事件回调
    label.highlightTapAction = ^(UIView *containerView, NSAttributedString *text, NSRange range, CGRect rect) {
        NSLog(@"tap text range:...");
    };
    label.highlightLongPressAction = ^(UIView *containerView, NSAttributedString *text, NSRange range, CGRect rect) {
        NSLog(@"long press text range:...");
    };
    
    @UITextViewDelegate
    - (void)textView:(YYTextView *)textView didTapHighlight:(YYTextHighlight *)highlight inRange:(NSRange)characterRange rect:(CGRect)rect {
        NSLog(@"tap text range:...");
    }
    - (void)textView:(YYTextView *)textView didLongPoressHighlight:(YYTextHighlight *)highlight inRange:(NSRange)characterRange rect:(CGRect)rect {
        NSLog(@"long press text range:...");
    }


### 图文混排

	NSMutableAttributedString *text = [NSMutableAttributedString new];
	UIFont *font = [UIFont systemFontOfSize:16];
	NSMutableAttributedString *attachment = nil;
	
	// 嵌入 UIImage
	UIImage *image = [UIImage imageNamed:@"dribbble64_imageio"];
	attachment = [NSMutableAttributedString yy_attachmentStringWithContent:image contentMode:UIViewContentModeCenter attachmentSize:image.size alignToFont:font alignment:YYTextVerticalAlignmentCenter];
	[text appendAttributedString: attachment];
	
	// 嵌入 UIView
	UISwitch *switcher = [UISwitch new];
    [switcher sizeToFit];
	attachment = [NSMutableAttributedString yy_attachmentStringWithContent: switcher contentMode:UIViewContentModeBottom attachmentSize:switcher.size alignToFont:font alignment:YYTextVerticalAlignmentCenter];
	[text appendAttributedString: attachment];
	
	// 嵌入 CALayer
	CASharpLayer *layer = [CASharpLayer layer];
	layer.path = ...
	attachment = [NSMutableAttributedString yy_attachmentStringWithContent: layer contentMode:UIViewContentModeBottom attachmentSize:switcher.size alignToFont:font alignment:YYTextVerticalAlignmentCenter];
	[text appendAttributedString: attachment];
	
	
### 异步排版和渲染
    
    // 如果你在显示字符串时有性能问题，可以这样开启异步模式：
    YYLabel *label = ...
    label.displaysAsynchronously = YES;
    
    // 如果需要获得最高的性能，你可以在后台线程用 `YYTextLayout` 进行预排版： 
    YYLabel *label = [YYLabel new];
    label.displaysAsynchronously = YES; //开启异步绘制
    label.ignoreCommonProperties = YES; //忽略除了 textLayout 之外的其他属性
    
    dispatch_async(dispatch_get_global_queue(DISPATCH_QUEUE_PRIORITY_DEFAULT, 0), ^{
        // 创建属性字符串
        NSMutableAttributedString *text = [[NSMutableAttributedString alloc] initWithString:@"Some Text"];
        text.yy_font = [UIFont systemFontOfSize:16];
        text.yy_color = [UIColor grayColor];
        [text yy_setColor:[UIColor redColor] range:NSMakeRange(0, 4)];
 
        // 创建文本容器
        YYTextContainer *container = [YYTextContainer new];
        container.size = CGSizeMake(100, CGFLOAT_MAX);
        container.maximumNumberOfRows = 0;
        
        // 生成排版结果
        YYTextLayout *layout = [YYTextLayout layoutWithContainer:container text:text];
        
        dispatch_async(dispatch_get_main_queue(), ^{
            label.size = layout.textBoundingSize;
            label.textLayout = layout;
        });
    });

### 文本容器控制

	YYLabel *label = ...
	label.textContainerPath = [UIBezierPath bezierPathWith...];
	label.exclusionPaths = 	@[[UIBezierPath bezierPathWith...];,...];
	label.textContainerInset = UIEdgeInserMake(...);
	label.verticalForm = YES/NO;
    
    YYTextView *textView = ...
	textView.exclusionPaths = 	@[[UIBezierPath bezierPathWith...];,...];
	textView.textContainerInset = UIEdgeInserMake(...);
	textView.verticalForm = YES/NO;
    
### 文本解析
	// 1. 创建一个解析器
	
	// 内置简单的表情解析
    YYTextSimpleEmoticonParser *parser = [YYTextSimpleEmoticonParser new];
    NSMutableDictionary *mapper = [NSMutableDictionary new];
    mapper[@":smile:"] = [UIImage imageNamed:@"smile.png"];
    mapper[@":cool:"] = [UIImage imageNamed:@"cool.png"];
    mapper[@":cry:"] = [UIImage imageNamed:@"cry.png"];
    mapper[@":wink:"] = [UIImage imageNamed:@"wink.png"];
    parser.emoticonMapper = mapper;
	
	// 内置简单的 markdown 解析
	YYTextSimpleMarkdownParser *parser = [YYTextSimpleMarkdownParser new];
    [parser setColorWithDarkTheme];
    
    // 实现 `YYTextParser` 协议的自定义解析器
    MyCustomParser *parser = ... 
    
    // 2. 把解析器添加到 YYLabel 或 YYTextView
    YYLabel *label = ...
    label.textParser = parser;
    
    YYTextView *textView = ...
    textView.textParser = parser;


### 更多示例
查看演示工程 `Demo/YYTextDemo.xcodeproj`:

<img src="https://raw.github.com/ibireme/YYText/master/Demo/DemoSnapshot/text_path.gif" width="320">
<img src="https://raw.github.com/ibireme/YYText/master/Demo/DemoSnapshot/text_markdown.gif" width="320">
<br/> <br/>
<img src="https://raw.github.com/ibireme/YYText/master/Demo/DemoSnapshot/text_vertical.gif" width="320">
<img src="https://raw.github.com/ibireme/YYText/master/Demo/DemoSnapshot/text_paste.gif" width="320">

    
安装
==============

### Cocoapods

1. 在 Podfile 中添加 `pod "YYText"`。
2. 执行 `pod install` 或 `pod update`。
3. 导入 \<YYText/YYText.h\>。


### Carthage

1. 在 Cartfile 中添加 `github "ibireme/YYText"`。
2. 执行 `carthage update --platform ios` 并将生成的 framework 添加到你的工程。
3. 导入 \<YYText/YYText.h\>。


### 手动安装

1. 下载 YYText 文件夹内的所有内容。
2. 将 YYText 内的源文件添加(拖放)到你的工程。
3. 链接以下 frameworks:
    * UIKit
    * CoreFoundation
    * CoreText
    * QuartzCore
    * Accelerate
    * MobileCoreServices
4. 导入 `YYText.h`。


文档
==============
你可以在 [CocoaDocs](http://cocoadocs.org/docsets/YYText/) 查看在线 API 文档，也可以用 [appledoc](https://github.com/tomaz/appledoc) 本地生成文档。


系统要求
==============
该项目最低支持 iOS 6.0。


许可证
==============
YYText 使用 MIT 许可证，详情见 LICENSE 文件。
