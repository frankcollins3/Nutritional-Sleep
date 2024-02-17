# Nutritional-Sleep
The sleep themed, sheep themed fasting tracker &amp; fan page 
A0CB51 // found the green for this app with a typo for journaldojo's brown: #A06B51


zZz this app is about rest and healing. 


heart-shaped-cursor: CSS($('*'), 'cursor', `url('/water_img/heart.png'), auto`)       


// was going to write this as the commit but it's very important to know so keeping it internal:
this app, like waterapp/WAPP/fill_cont:

simple, whimsical design that expresses time based functionality

both a water app and fasting app will have:
start_time, end_time, reminder related functionality.

there's seemingly little to implement:
 so much space can be lent to large images.

original WAPP/water app which I didn't design
makes use of a settings bar that pops up as 1 of navbar icons.

when the calendar pops up half the middle screen just says:
"Pick a Highlighted Day"

The dashboard that is the current data for current water cycle
or in nutritional sleep iteration would be current fast.

dashboard & calendar will be almost the whole app.
// GotchaSheep -----> TomaGatchi knockoff: 
1:sheep.feed() && tend heart bar levels. [might link this to "food list" and allow human to feed sheep the food it would've eaten while fasting]
2 human stays happy fasting. Sheep helps human.


bookmarking a message to myself that in noticing:

* * Always Ask ! : is this a need-a-calendar or not kind of App. How can Component-Composition or Context be used with the data tables or state in the app ? * * 

mine-nugget-ts:
// no use for calendar.
page 1: displays every piece of API data from fs.json or postgres besides the data.strain.parentGeneticsOfStrain
page 2: creates a simple guessing game out of providing the data.strain.parentData withHeld from display from page. User can guess child based on parents.
page 3: search page with magnifying glass. toggle between seeing reviews/likes from other users with other strains. 

<Context>
 
 RegexContext
 *** 3: RstringAfterPeriod || mSplitAtDot           provide first Letter to indicate whether Replace or Match is used for that regex.  (also i.e.) -> asteriskSplit: name splits    ***
type RegexContextType = {
    RstringAfterPeriod: RegExp;
    RreturnLettersAthruZ: RegExp;
    RreturnNumbers: RegExp;
    RhasCaps: RegExp;
    RhasNums: RegExp;
    RnoWhiteSpace: RegExp;
    MsplitAtDot: RegExp;
  }
 
 ImageContext

PromisesContext.tsx for redux and any other Promises 
 
might use the fasting data as an <App-Wrapping-Context>


AM | PM timing: 
{time <= 12 ? time : time - 12}:00 {time < 12 ? 'am' : 'pm'}


To render fasting data make an array that has [progress] and weekly status. Loop over the data array and check for progress and status to determine whether UI shows successful or not fast 
`  const renderSchedule = () => {
    
    return HYDRO_SCHEDULE.map((time:any, index:number) => (
      
      <ConnectedReminder
        key={index}
        time={time}
        amt={(hydroIntake / hydroSchedule.length) * (index + 1)}
        amtper={hydroIntake / hydroSchedule.length}
        percent={Math.floor(
          (((hydroIntake / hydroSchedule.length) * (index + 1)) / hydroIntake) *
            100 -
            1
        )}
        index={index}
        // handleClick={handleClick}
        status={status}
        setStatus={setStatus}
        disabled={disabled}
        setDisabled={setDisabled}
      />
    ));`
