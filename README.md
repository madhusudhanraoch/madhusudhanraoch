I am trying to update github "SwipeCellKit/SwipeCellKit" for Carthage in xcode 13 beta 5 but Failed .

*** Fetching SwipeCellKit
*** Checking out SwipeCellKit at "2.7.1"
*** xcodebuild output can be found in /var/folders/x8/dnk5cymd3wz1w_ccvz755pr00000gq/T/carthage-xcodebuild.wogWsL.log
*** Building scheme "SwipeCellKit" in SwipeCellKit.xcworkspace
Build Failed
	Task failed with exit code 65:
	/usr/bin/xcrun xcodebuild -workspace /Users/safuan/Desktop/NinthList/Carthage/Checkouts/SwipeCellKit/SwipeCellKit.xcworkspace -scheme SwipeCellKit -configuration Release -derivedDataPath /Users/safuan/Library/Caches/org.carthage.CarthageKit/DerivedData/13.0_13A5212g/SwipeCellKit/2.7.1 -sdk iphoneos ONLY_ACTIVE_ARCH=NO CODE_SIGNING_REQUIRED=NO CODE_SIGN_IDENTITY= CARTHAGE=YES archive VALIDATE_WORKSPACE=NO -archivePath /var/folders/x8/dnk5cymd3wz1w_ccvz755pr00000gq/T/SwipeCellKit SKIP_INSTALL=YES GCC_INSTRUMENT_PROGRAM_FLOW_ARCS=NO CLANG_ENABLE_CODE_COVERAGE=NO STRIP_INSTALLED_PRODUCT=NO (launched in /Users/safuan/Desktop/NinthList/Carthage/Checkouts/SwipeCellKit)

This usually indicates that project itself failed to compile. Please check the xcodebuild log for more details: /var/folders/x8/dnk5cymd3wz1w_ccvz755pr00000gq/T/carthage-xcodebuild.wogWsL.log


Users/safuan/Desktop/NinthList/Carthage/Checkouts/SwipeCellKit/Source/SwipeActionsView.swift:10:36: warning: using 'class' keyword to define a class-constrained protocol is deprecated; use 'AnyObject' instead
protocol SwipeActionsViewDelegate: class {
                                   ^~~~~
                                   AnyObject
/Users/safuan/Desktop/NinthList/Carthage/Checkouts/SwipeCellKit/Source/SwipeCollectionViewCellDelegate.swift:13:50: warning: using 'class' keyword to define a class-constrained protocol is deprecated; use 'AnyObject' instead
public protocol SwipeCollectionViewCellDelegate: class {
                                                 ^~~~~
                                                 AnyObject
/Users/safuan/Desktop/NinthList/Carthage/Checkouts/SwipeCellKit/Source/SwipeTableViewCellDelegate.swift:13:45: warning: using 'class' keyword to define a class-constrained protocol is deprecated; use 'AnyObject' instead
public protocol SwipeTableViewCellDelegate: class {
                                            ^~~~~
                                            AnyObject
/Users/safuan/Desktop/NinthList/Carthage/Checkouts/SwipeCellKit/Source/SwipeController.swift:11:35: warning: using 'class' keyword to define a class-constrained protocol is deprecated; use 'AnyObject' instead
protocol SwipeControllerDelegate: class {
                                  ^~~~~
                                  AnyObject

Command CompileSwiftSources failed with a nonzero exit code
** ARCHIVE FAILED **


The following build commands failed:
	CompileSwift normal armv7 (in target 'SwipeCellKit' from project 'SwipeCellKit')
	CompileSwiftSources normal armv7 com.apple.xcode.tools.swift.compiler (in target 'SwipeCellKit' from project 'SwipeCellKit')
	CompileSwiftSources normal arm64 com.apple.xcode.tools.swift.compiler (in target 'SwipeCellKit' from project 'SwipeCellKit')
