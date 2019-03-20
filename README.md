This page is dedicated to the distribution of the data used for the paper: 

“Drive Me Not – GPS Spoofing Detection via Cellular Network”, by Gabriele Oligeri, Savio Sciancalepore, Omar Adel Ibrahim and Roberto Di Pietro, from Hamad Bin Khalifa University (HBKU) - College of Science and Engineering (CSE) - Division of Information and Computing Technology (ICT), accepted at the 2019 ACM Conference on Security and Privacy in Wireless and Mobile Networks (ACM WiSec 2019). 

In our paper, these data have been used to detect ongoing GPS spoofing activities on a target moving device, such as a car or a truck.

They have been acquired using a a smartphone running the Android Operating System version 8.1.0, kernel version 4.4.95+, equipped with a MT6739 Quad Core processor running at 1.3Ghz, 8GB of ROM memory and 1GB of RAM memory. The smartphone features two Subscriber Identication Module (SIM) cards, thus being able to receive messages from two different operators at the same time. To orchestrate the acquisition, we have developed a dedicated Android application, able to collect information from both the cellular network and the GPS infrastructure at the same time. The user can specify a sampling period T; then, every T seconds, the application logs the information from the in-range Base Stations (BS) (by calling the Android method getAllCellInfo) and the current location of the smartphone (MT) obtained via the GPS (using the Android methods requestLocationUpdates and getLastKnownLocation of the LocationManager library).

Then, it generates a log-file with all the information.

Each file contains the following columns:

GPS_lat, GPS_lon: latitude and longitude of the mobile node
Time: absolute time (microseconds)
CID, LAC, MCC, MNC: Base station information
dBm: Received Signal Strength
