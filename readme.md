# Amazon Alexa Loadshedding Skill

This is a rough POC of an Amazon Alexa skill using the EskomSePush beta API.

The skill is invoked with the phrase `Alexa, ask my fancy power schedule`.

Alexa does not support the word `load` in a custom skill, and hence the work load shedding cannot be used to invoke the skill.

Once the skill is launched it gives you the load shedding schedule for a single hardcoded suburb based on the results of the `area search` method from the api.

The ideal use case is to link the Alex account to an EskomSePush user account when the skill is installed, using oauth, and to query the suburbs that the user has set-up in their EskomSePush app.


# Requirement and Installation

* You require access to the EskomSePush API and you need a corresponding API key.
* Your API key needs to go into a config.py file that is not checked into the repo for security reasons (indeed there are better ways to manage keys...).
* You need an [Amazon Developer Account](https://developer.amazon.com/en-US/docs/alexa/ask-overviews/create-developer-account.html).
* An Amazon echo device would be useful but you can use the virtual alternatives.
* To set-up the Skill, use the VS Code [Alexa Extension](https://developer.amazon.com/en-US/docs/alexa/ask-toolkit/vs-code-ask-skills.html)
* You will need to set-up a local Python environment, install the requirements, and follow the instructions in the extension to `import a local skill`, followed by the instructions of setting up to run it and test it locally in the emulator.
* Alternatively you can publish it to the cloud host and test from there.

These instruction are pretty spars and if its the first time setting up and Alexa Skill, it would be best to do a [tutorial](https://developer.amazon.com/en-US/docs/alexa/workshops/build-an-engaging-skill/get-started/index.html?sc_category=Paid&sc_channel=PSM&sc_campaign=evergreen&sc_publisher=GO&sc_content=Banner&sc_detail=GetStarted&sc_funnel=Awareness&sc_country=WW&sc_medium=Paid_PSM_evergreen_GO_Banner_GetStarted_Awareness_WW_Skill_Builders&sc_segment=Skill_Builders&gclid=Cj0KCQjwnbmaBhD-ARIsAGTPcfWlqWzYjGS8WeBgGycrmlZajuQNWQQzsSqC4o-91gZh8t_e0NcqX8kaAib-EALw_wcB) beforehand.
