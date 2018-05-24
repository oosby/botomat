# BOT-O-MAT
Use any language to complete this challenge. The implementation is up to you, it can be a console app or have a frontend.

- Collect a name and robot type from user.
- Instantiate a Good Robot of the type provided by the user with the name provied by the user
  - for example: Bipedal, Larry
- Instantiate a Bad Robot of the same type as Good Robot and has 'Bad-' prefixing the name
  - for example: Bipedal, Bad-Larry
- Set up methods on Good Robot to complete tasks from the provided list
- At random intervals have Bad Robot take a completed task and put it back on the todo list
  - for example: every 3rd completed task goes back on Good Bot's todo list

## Robot

### Good Robot
Good Robot completes tasks and removes them from the list when they are done (i.e. enough time has passed since starting the task).

### Bad Robot
Bad Robot is Good Robot's evil twin. It spies on Good Robot and randomly puts completed tasks back on the list.


## Tasks
Tasks have a description and an estimated time to complete.

```
[
  {
    description: 'do the dishes',
    eta: 1000,
  },{
    description: 'sweep the house',
    eta: 3000,
  },{
    description: 'do the laundry',
    eta: 10000,
  },{
    description: 'scrub the toilet',
    eta: 2000,
  },{
    description: 'peel and de-pith this orange',
    eta: 15000,
  },{
    description: 'make a sammich',
    eta: 7000,
  },{
    description: 'mow the lawn',
    eta: 20000,
  },{
    description: 'rake the leaves',
    eta: 18000,
  },{
    description: 'give the dog a bath',
    eta: 14500,
  },{
    description: 'bake some cookies',
    eta: 9000,
  },{
    description: 'wash the car',
    eta: 40000,
  },
]
```

## Types
```
{ 
  UNIPEDAL: 'Unipedal',
  BIPEDAL: 'Bipedal',
  QUADRUPEDAL: 'Quadrupedal',
  ARACHNID: 'Arachnid',
  RADIAL: 'Radial',
  AERONAUTICAL: 'Aeronautical'
}
```

## Iteration features
- Allow users to create multiple robots at one time
- create a leaderboard for tasks completed by each Good Robot
- Create a leaderboard for tasks put back by each Bad Robot
- Create tasks specific for each robot type
- Add persistance for tasks, bots and leaderboard stats
