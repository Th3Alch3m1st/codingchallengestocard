# Coding Challenge

## Demo
<a href="url"><img src="https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/screenshots/demo.gif" height="480" width="230" />
  
## Screenshots
<a href="url"><img src="https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/screenshots/sceen_home.png" height="480" width="230" />
<a href="url"><img src="https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/screenshots/screen_home_dark.png" height="480" width="230" />
<a href="url"><img src="https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/screenshots/screen_search.png" height="480" width="230" />
<a href="url"><img src="https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/screenshots/screen_search_result.png" height="480" width="230" />
<a href="url"><img src="https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/screenshots/screen_setting_selection.png" height="480" width="230" />
<a href="url"><img src="https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/screenshots/screen_settings.png" height="480" width="230" />

## Architecture
MVVM  with clean Architecture and moduler approch
  
## Third-party libraries
- Architecture Components: Lifecycle, ViewModel, Navigation, Safe Args
- UI component: Material
- Data Binding
- Coroutine, Flow
- Dependency injector: Hilt
- Networking: Retrofit, Moshi
- Glide: Image loading
- Unit testing: JUnit4, AssertJ, MockitoKotlin, Espresso Arch core testing (InstantTaskExecutorRule), Kotlinx coroutines test
- UI testing: Espresso
- Full list: https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/Dependencies.kt

## Project Structure
  <a href="url"><img src="https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/screenshots/projectStructure.png" height="466" width="485" />
  <a href="url"><img src="https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/screenshots/project_sructure.png" height="466" width="440" />
    
## Application Data flow
  <a href="url"><img src="https://github.com/Th3Alch3m1st/codingchallengestocard/blob/main/screenshots/flow.png" height="241" width="818" />  
    
## Approach
- ViewModel separate UI and Data layer. ViewModel allows data to survive configuration changes and improve testabilities.
- In City search different Grid spans are handled on orientation changes, In Portrait Mode 2 Grid item loaded and In Landscape mode 3 grid item loaded.
- In city search Filter class is used to search inside a list, it filters data from a large list asynchronously.
- Jetpack DataBinding to bind the layouts views and it's null safe.
- Use Kotlin DSL for gradle management - it helps better gradle management in multi module projects. And increase readability, provide code navigation and auto suggestions
- Write code maintaining SOLID principle
- User mapper class to convert network response into UI model
- Write Unit test and UI test to ensure app stability and performance
- Write some infix function to increase unit test readability
- Add documentation in UI test to explain test scenario and write short comment for unit test
