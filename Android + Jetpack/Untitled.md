```toc
```

The purpose of this entries is going to be record the learning process of making Android apps with Kotlin and Jetpack Compose.

## Some Kotlin things worth considering

`Lists` - are meant to contain the same type on all entries
`Sets` - are meant to not have any duplicates
- can sort itself by `toSortedSet()`
`Map` - <Key, Value>list with a customized index
- can use the keyword `to` ex: `1 to "Monday"`

## Manifest
[]
Describe the components of the application. Includes information about name, version, permissions and activities. 
This file is used to load and launch the app.

#### Sections:
1. Application section
	- name version and permissions 
2. Activity section
	- info about the activity
	- an activity is a screen that the user can see and interact with
3. Service section
	- info about app services
	- a service is a background task, that runs even when the user is not interacting with the app
4. Receiver section
	- info about the receiver
	- a receiver is a component that receives broadcast messages from the system
5. Provider section
	- info about the provider
	- component that can provide data to other components