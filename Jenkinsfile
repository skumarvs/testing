pipeline {
  agent any
  parameters {
choice(name: 'food_choice', 
	choices: 'pizza\nburger\nTortitas\nchips',
	description: 'Test Drop Down?')
booleanParam(name: 'canEat',
	 defaultValue: true,
	description: 'Check box Parameter')
String(name: 'teststringparam',
	defaultValue: 'defaultstringvalue',
	description: 'String description for test!!!')
}	
  stages {
    stage('Build') {
      steps {
        echo 'hi sid'
	echo " Going to eat ${params.food_choice}"
	echo "Is Eatable ${params.canEat}"
	echo "Eat this String ${params.teststringparam}"
      }
    }
  }
}