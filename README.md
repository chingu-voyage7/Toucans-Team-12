# Toucans-Team-12
####### Wakaru ####### | Voyage-7 | https://chingu.io/

	#1 Project definiton:

		Wakaru is a web app allowing users to search for kayaking routes.

		MVP:
		Allows finding a route near given location and adding new routes.

		Add-ons:
			User auth.
			User "wish-list" - saving routes.
			Route filtering.
			Route reviews.
			Route charting on-the-go (using cellphone GPS).
			Difficulty color mapping.	
			Weather forecast for given date around route.
			Route sharing (email, social media).

	#2 User cases:

		//Wakaru allows users to search for kayaking routes.

			User: types location into @search field@.
			App: @Map@ displays routes around that location.

			User: Clicks on a route.
			App: Displays @route details@ + displays @points of interest@ along the route.
					#Route details:
						- Route rating
						- Difficulty rating
						- Start/End Point Address
						- Route length (distance travelled, time to complete)
						- User reviews (route rating + difficulty rating + comment)


		//Wakaru allows users to filter routes in an area.

			User: Opens @Filter tab@.
			App: Display @Filter options@.
					#Filter options:
						- Rating
						- Difficulty
						- Length (distance travelled)
						- Length (time to complete)
						- Search radius (distance in km from specified location to look in)

			User: Selects filters, clicks @Confirm button@.
			App: Hide filtered routes from current view on @Map@.


		//Wakaru allows users to add new routes.

			User: Clicks @Sign in@, input credentials, clicks OK.
			App: Authenticates user. Displays additional @Add route@ button on map.

			User: Navigates to area, clicks @Add route@.
			App: Opens @Map@ in editing mode. Shows @Drawing tools panel@.
					#Drawing tools panel:
						- Draw polyline.
						- Add POI.

			User: Confirms route by click @Complete button@.
			App: Displays @Route details tab@ asking user to input initial rating, initial difficulty. 

			User: Confirms @route details@.
			App: Encodes data in JSON and sends to Firebase.


	#3 User target group:

		//Wakaru user:

				Based on: https://www.breakingblueresearch.com/documents/kayaking-canoeing.pdf
					- 77% Male
					- 55% Between 35-54 years old
					- 30% want to relax, 30% want to explore and challenge themselves, only 13% hardcore sportsmen.
					- 40% go paddling few times a year or less, other 40% go very often.
					- Very conscious of safety - weather forecasts, route sharing.

######################
