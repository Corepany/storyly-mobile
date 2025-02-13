# Release Notes
### 1.11.1
* added isTestMode field to StorylyInit to show test story groups, check [Test Mode](https://integration.storyly.io/ios/test-mode.html)
* improved status bar handling for specific devices, [#88](https://github.com/Netvent/storyly-mobile/issues/88)

### 1.11.0
* added image component for interactive stories
* added video component for interactive stories
* IMPORTANT! removed advertising id(idfa compatibility for iOS 14.5) usage
* IMPORTANT! removed url field from StoryMedia
* IMPORTANT! renamed rawValue of StorylyEvent to stringValue

### 1.10.1
* fixed a crash on fallback scenarios

### 1.10.0
* added product tag component for interactive stories
* improved story area usage 
* fixed pinned story groups ordering 
* fixed emoji rendering on text interactive components
* fixed font rendering on text interactive components

### 1.9.5
* fixed crash on iOS 12 devices, NSInternalInconsistencyException, [#72](https://github.com/Netvent/storyly-mobile/issues/72)

### 1.9.4
* fixed crash on iOS 12 devices, [#72](https://github.com/Netvent/storyly-mobile/issues/72)

### 1.9.3
* fixed crash runtime segmentation changes [#58](https://github.com/Netvent/storyly-mobile/issues/58)

### 1.9.2
* added actionUrlList to Story data
* fixed crash if storyHeaderIconIsVisible=false used [#52](https://github.com/Netvent/storyly-mobile/issues/52)

### 1.9.1
* added support for interactive components without titles
* added animation to swipe up icon and text
* added dynamic changes for storyly list updates
* added set language support for specific languages (TR, EN, RU, ES, DE, FR)
* added thematic icon support for story groups

### 1.9.0
* added Interactive VOD feature
* added vertical, horizontal and custom placement support for emoji component
* improved cube animation during transitions
* improved interactive layer rendering
* IMPORTANT! changed storylyActionClicked signature(removed return type)

### 1.8.9
* improved story header animation during long press
* improved cache flow

### 1.8.8
* added Story header animation during long press
* improved Xcode12.2 support(Swift 5.3.1 support)

### 1.8.7
* added storylyEvents method to StorylyListener
* added 'seen' field to StoryGroup and Story
* improved Xcode12 support(Swift 5.3 support)

### 1.8.5
* improved initialization handling

### 1.8.4
* added StoryGroupListStyling to support customization of story group list view, added 'storyGroupListEdgePadding' as storyboard and programmatic attributes
* moved 'storyGroupListPaddingBetweenItems' to StoryGroupListStyling
* improved share link generation
* fixed story header font update bug
* improved swipe down close animation for newer iPhone devices

### 1.8.3
* improved UI components for better iOS14 support
* improved status bar management

### 1.8.2
* added 'storyItemTextFont' as storyboard and programmatic attribute to support custom font for story title
* added 'isCloseButtonVisible' attribute to StoryHeaderStyling and 'storyHeaderCloseButtonIsVisible' as storyboard and programmatic attribute for visibility option of close button
* added 'showExternalActionView' and 'dismissExternalActionView' methods to support external custom view to show and dismiss while stories are being shown
* added 'storylyLoadingView' attribute to support external custom loading view instead of using default loading view

### 1.8.0
* added rating component for interactive stories
* added language support for en, tr, de, fr, ru, es locales
* added StoryGroupIconStyling to support custom size story groups, added 'storyGroupIconWidth', 'storyGroupIconHeight', 'storyGroupIconCornerRadius' and 'storyGroupPaddingBetweenItems' as storyboard and programmatic attributes
* added StoryGroupTextStyling for visibility handling of elements, added 'storyGroupTextIsVisible' as storyboard and programmatic attribute
* added StoryHeaderStyling for visibility handling of elements, added 'storyHeaderIconIsVisible', 'storyHeaderTextIsVisible' as storyboard and programmatic attributes
* added runtime update feature for StorylyInit's segmentation parameters

### 1.7.3
* fixed compile issue due to swift backward compatibility

### 1.7.2
* added storylyUserInteracted(storylyView: StorylyView, storyGroup: StoryGroup, story: Story, storyComponent: StoryComponent) callback
* improved events for better analysis

### 1.7.0
* added countdown component for interactive stories
* added share feature to stories
* removed close button from stories

### 1.6.2
* improved event payload for better analysis

### 1.6.1
* added id field to Story and StoryGroup classes
* added iconImageUrl to StoryGroup class
* added openStory(storyGroupId: Int, storyId: Int?) method
* added thumbnail image to video stories
* improved event payload for better analysis

### 1.6.0
* added quiz component for interactive stories
* removed use_frameworks! constraint for CocoaPods integrations

### 1.5.5
* fixed compile issue due to swift backward compatibility (issue: inheritance from non-protocol type 'UIView')

### 1.5.4
* added 'xlarge' story group size 
* added storyGroupIconForegroundColors method for 'xlarge' story groups gradient layer
* added storyGroupTextTypeface method
* added 'customParameter' parameter to StorylyInit to pass customized field for users

### 1.5.3
* fixed a bug in external data

### 1.5.1
* added frame parameter to StorylyExternalViewProvider callback to support better sizing

### 1.5.0
* added interactive stories support for poll
* updated placement of emoji reaction view

### 1.4.0
* added client side ad insertion flow
* improved StorylyInit and StorylySegmentation class initializers for ObjC
* added BUILD_LIBRARY_FOR_DISTRIBUTION as compile option to support backward Swift compatibility

### 1.3.2
* IMPORTANT! changed StorylyInit class definitions, please check README
* fixed a rare bug during transitions
* fixed crash during empty story group list scroll

### 1.3.0
* IMPORTANT! removed storylyId with storylyInit parameter, please check README
* IMPORTANT! changed openStory method signature, please check README
* added setExternalData api to extend personalized usage, please check Advanced Topics
* added segmentation of story groups
* added dynamic/runtime segmentation of story groups, please check Advanced Topics
* added 'large'(default one) and 'small' story group size 

### 1.2.2
* add dependency to podspec

### 1.2.1
* fix crash during deeplink openings

### 1.2.0
* Performance improvements on story transitions
* Added capability to open stories using deeplink generated from dashboard
* [Segmentify](https://www.segmentify.com/) integration to show personalized stories to users

### 1.1.0
* add interactive stories support for custom button action, text and emoji reaction

### 1.0.2
* improvements on placement for different device ratio including tablets
* improvement on orientation change handling for iPads

### 1.0.1
* improvements on placement for different device ratios
* fix pin icon bug

### 1.0.0
* IMPORTANT! change storylyLoad callback signature, please check README
* IMPORTANT! change storylyLoadFailed callback signature, please check README
* add storylyStoryPresented and storylyStoryDismissed callbacks
* rename StorylyData to StoryData
* improvements on pull down and overscroll animations

### 0.0.22
* improvements on notch handling
* improvements on dismiss animation for iPhoneX
* fix StorylyView constructors' visibility modifier issue

### 0.0.21
* fix gesture handling for overscroll dismiss

### 0.0.20
* add pull down for close story
* add animation to dismiss action
* add multiple instance support
* fix video buffer issue
* significant improvements on performance

### 0.0.19
* improvements and modications

### 0.0.18
* rename appId to storylyId
* improvements on video story

### 0.0.15
* improvements for iPhoneX

### 0.0.14
* add UI customization APIs, please check README for details
* add pinned story flow
* improve story loading for better UX
* change action view icons

### 0.0.13
* add BUILD_LIBRARY_FOR_DISTRIBUTION setting
* improvements on gestures

### 0.0.11
* add skeleton view for loading cases
* improvements on gestures
* enable bitcode generation

### 0.0.10
* change storylyActionClicked delegate signature 
* ui changes
* fix video story playback

### 0.0.9
* add pause/resume API
* add story title

### 0.0.8
* add cubic animation to story transititon
* handle orientation changes

### 0.0.7
* add refresh API
* add story seen state handling
* add duration configuration from backend; current configuration is 7sec for image type stories, 15sec for video types

### 0.0.6
* add storylyActionClicked deleagate
* Swift 5.1 compatibility
