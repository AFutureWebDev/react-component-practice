
### Intro
The purpose of this project is to practice coding React components. We will use our knowledge of creating functional components where each component is coded in its own file. We are also going to experience what might really happen on the job. You may be tasked with working an existing website in which all the html is crammed into one file. Your job is to implement React and decide how you can organize the existing html into components. In this project you are told what the components should be but in real life you would have to decide this for yourself.

### Setup
* Use http-server or similiar to serve the index.html file from the public folder

### Create components
* In App.js, do a find for comments that look like `{/*   <TopNav>   */}  {/*   </TopNav>   */}`
* Search for the name of the component you are attempting to make
* This will indicate where the component should start and end
* Or use the expand/collapse feature of the editor to find the start and end
* Cut out the code between the comments and put in its own file
* Create .js files for each component. Make sure to name it the same as the component.
* Decide what is in the component that should not be hard coded
* Remove hard coded info and define what props are needed by this component to show dynamic information
* Create the component files in /js/src/components
* Add script tag to index.html to include the component in the web page
* Make sure the script tags are in the correct order


### Components
* TopNav
* SideNav
* Comments
* Tasks
* Orders
* Tickets
* AreaChart
* DonutChart
* TasksPanel
* TransactionsPanel
* MessagePreview (which is in TopNav)
* DateTime (which is in MessagePreview)
* TaskItem (which is in TaskPanel)
* TransactionRow (which is in TransactionsPanel)

### Use components where appropriate
* Wherever you cut out the html, you need to replace it with the tag of the component
* Replace the comments with the actual usage of the components (custom element) `<TopNav />`

### Props
* Pass the newComments prop from App to Comments
* Pass the newTasks prop from App to Tasks
* Pass the newOrders prop from App to Orders
* Pass the tickets prop from App to Tickets

* Pass the orders prop from App to TransactionPanel
* Pass the messages prop from App to TopNav
* Pass the tasks prop from App to TaskPanel

### Use Props
* TaskItem should use the task prop to populate the task name and the date
* TransactionRow should use the order prop to populate the `<td>` s
* MessagePreview should use the message prop to populate the name, date and message text

### Mapping
* TasksPanel - map the array of "tasks" into array of TaskItem's. Pass one task into TaskItem
* TopNav - map the array of "messages" into array of MessagePreview's. Pass one message into MessagePreview
* TransactionPanel - map the array of "orders" into array of TransactionRow's. Pass one order into TransactionRow


