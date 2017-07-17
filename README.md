## An app that assists users with their fashion choices

This app allows users to upload a photo of an outfit for users to rate by swiping left or right to show their thoughts. This way, the user can always go out knowing that they have an amazing outfit that is approved by people who know style.

### To do:
 *  Need to add code to ensure same photo isn't voted on twice by single user
   * If it is, do not allow voting to occur (Make sure same for reporting)
 * Either have a "last viewed" or "photos viewed" section in db, or have a timestamp which will show until what point user has seen photos. This will be useful if starting from oldest to newest.
 * Another option is to have from newest to older, but will need to find another way to ensure previously rated photos will not show up.
   * Better yet show everything, just don't allow user's vote (or report) on own photo to count. Show 15 photos at a time or whatever is left in the array of total photos (whichever is least). 
 * Come up with new clever name
 * Put app on Google play
 * Create tests
 * Improve layout
 * Handle screen rotations savedinstancestate on ALL activities
 * Create Terms of Service
 * Localize
 * Make material design
    * Make tablet layout
 * Have interstitial ads show up after x - swipes

### Done
 * Set up swipe card layout
 * Set up sign in and sign out using Firebase AUTH and Firebase UI
 * Choose Material Design Color Scheme
 * Set up Firebase ads
 * Have photo upload to Firebase storage
 * Set up Firebase database
   * Db structure
    * [user|photo urls]
    * [photo urls|likes|dislikes|reports|usernames]
 * Set up photo functionality
 * Create layout for new photo creation
 * Allow reporting of photos
 * Make a progress bar for user to see photo upload progress
 * Have my account section with photos
 * Set up rating system for user likes or dislikes
 * Create catchy launcher icon 

### Known bugs/todo/ to fix:
 * Photos load slowly and not always
 * On click thumbs disappear, numbers do not
 * User can vote twice on same photo
 * If activity is exited upload fails
 * Don't allow users to vote on own photos
 * Shows all photos in home screen when it should show all photos except user photos in home screen
 * Shows all photos in my photos screen when it should show only user photos in home screen
 * Gets EVERY SINGLE PHOTO. Needs to be fixed as this is not yet ready to scale.
 
### Possible features:
* If enough users are not being rated then allow for only one photo to be uploaded/ rated for free and then future photos will be on a per-rate basis where 1 rate = 1 new photo uploaded
* Allow following other users
   * This will add a field to the user part of the database which will be followed users. Possibilities for this are:
     * The app will push photos from the followed users to the front of the list of photos to rate.
     * Dedicated section to followed users (like with youtube subscriptions)
   * Add number of followers to user part of database
   * Add search user
   * Add profile photos
 * Add option to skip or indifferent view of style
 * Have local database so that "my photos" section will load faster
 * Make text dynamically size to view






###### Credit to
* Diolor for SwipeCards Layout
* Google for the Google Libraries used
* Ben Manes for the Dependency Updates library
