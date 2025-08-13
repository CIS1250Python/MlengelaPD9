The program - GEO-POINTS WITH A FILE - demonstrates how to define a class with a file. It is going to change the GeoPoint Class of the last program: [MlengelaPD8](https://github.com/CIS1250Python/MlengelaPD8/blob/main/MlengelaDP8.zip), instead of only working with
Two points: the project will read a list of five or more points from a file. 

1. We create a file that has the data for at least five points. Notepad is used to make a file.
2. Each line in the file should have each point's lat and lon coordinates and a description. It could look like this:
   * 35.0714,106.6289,Main Campus
   * 35.0998,104.0639,Montoya
   * 35.2328,106.6630,Rio Rancho
   * 35.0856,106.6493,STEMULUS Center
   * 35.1836,106.5939,ATC
   ( Note: The "Points.txt" file attached to the assignment can be used instead of creating your own file)
3. In the main part of your program, do the following:
    * a.Create a list that you will use to collect the points. Something like pointsList = [].
    * b.Read the points from a file.
    * c.As you read lat, lon, and description from the file, use those values to create a point and add that point to a List. Something like:
                   newPoint = GeoPoint(lat, lon, description)
                   pointsList.append(newPoint)
    * d. Inside the "Do another(y/n)?" loop do the following:
        i). Ask the user for their location
               ii). Create a point to represent the user's location.
               iii). Iterate through the points list created from the file and find the closest point the user is to.
                iv). Tell the user which point they are closest to in the format:
                   You are closest to < description>, which is located at <point's lat, lon coordinates>
                 v). Ask "Do another(y/n) and loop if they respond with 'y'

