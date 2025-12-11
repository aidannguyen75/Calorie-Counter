# Calorie Counter
# Description of Application 
This project is a android application created in Android-Studio built using Java, with intended prupoose is to be able to provide the users with a method to be able to track and maintain their caloric goals throiughg input of various food items, which the user will store and record the items name, caloric vaLue, and quantoty of item, to meet a set caloric goal throughout the day. The appllication will also havbe access to a calendar feature which will allowq the user to be able to view previous entries on previous days and keep a tab on wether their goals have or have not been met. Furthermore the application also provides the use of a notificatin feature which the user could use, enabling them to be able to set reminders throughout the day and allow custom messges to be sent to remind trhem of any specific needs that need to be attended too. 

#File Structuere 
app/
 └── java/com.example.caloriecounter/
 
       ├── ui/
       │   ├── Goals/
       │   │   └── CustomCalendarView.java 
       |   |   ├── GoalsViewModel.java
       │   │   └── GoalsFragment.java
       |   |   |___DayDetailFragment.java
       |   | OverView/
       │   │   ├── EntreiesAdapter.java
       │   │   └── OverviewFragmeent.java
       |   |   |__ OverviewViewModel.java
       │   ├── Reminders/
       │   │   ├── ReminderFragment.java
       │   │   ├── ReminderManager.java
       │   │   ├── ReminderReceiver.java
       │   │   ├── ReminderService.java
       │   │   └── NotificationHelper.java 
       |   |   |___RemidersViewModel.java

These files contain the codes implemented disregarding other files where the User Interface was created with each file corresponding to the 3 main pages of the applicatin that being the Goals Page where the user sets their caloric intake goal with some hard coded presets that the user may use if they are uncertain about what goal they should follow.
#Caloric Presets
private void initializePresets() {

        presets = new ArrayList<>();
        presets.add(new CaloriePreset("Sedentary Adult Male", 2000, 2500));
        presets.add(new CaloriePreset("Sedentary Adult Female", 1600, 2000));
        presets.add(new CaloriePreset("Active Adult Male", 2400, 3000));
        presets.add(new CaloriePreset("Active Adult Female", 2000, 2400));
        presets.add(new CaloriePreset("Teen Male (14-18)", 2400, 2800));
        presets.add(new CaloriePreset("Teen Female (14-18)", 1800, 2400));
        presets.add(new CaloriePreset("Child (9-13)", 1600, 2200));
        presets.add(new CaloriePreset("Very Active Male", 2800, 3500));
        presets.add(new CaloriePreset("Very Active Female", 2200, 2800));
        presets.add(new CaloriePreset("Weight Loss Male", 1500, 1800));
        presets.add(new CaloriePreset("Weight Loss Female", 1200, 1500));
        presets.add(new CaloriePreset("Weight Gain Male", 2500, 3200));
        presets.add(new CaloriePreset("Weight Gain Female", 2000, 2600));
