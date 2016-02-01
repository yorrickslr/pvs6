# puvs6
Parallele und verteilte Systeme - Übung 6


Das verwendete System hat folgende Spezifikationen:  
>   CPU:    AMD Athlon II x2 240  
>   RAM:    8Gb DDR3 @1333MHz  
>   GraKa:  Palit GTX 560 OC  
>   MoBo:   MSI 970 GAMING  
>   SSD:    OCZ Vector 150 @6GB/s  

var0 -> Version aus Übung 5  
Zeit:  
Matrix sizes C[1000][1000] = A[1000][1000] x B[1000][1000]  
Running serial algorithm...  
Checking results... ok.  
Showing stats...  
   serial runtime = 9.448016  
   OpenCL runtime = 0.223518  
   Speedup = 42.269541  

var1 -> Nutzung einer temporären lokalen Variable für die Berechnung der einzelnen Elemente  
Zeit:  
Matrix sizes C[1000][1000] = A[1000][1000] x B[1000][1000]  
Running serial algorithm...  
Checking results... ok.  
Showing stats...  
   serial runtime = 9.571843  
   OpenCL runtime = 0.291683  
   Speedup = 32.815876  

var2 -> Da es in unserer Version keine äußeren Schleifen mehr gibt, entfällt diese Implementierung  
var3 -> Statt A wird privater Speicher tempA genutzt  
Zeit:  
Matrix sizes C[1000][1000] = A[1000][1000] x B[1000][1000]  
Running serial algorithm...  
Checking results... ok.  
Showing stats...  
   serial runtime = 10.664608  
   OpenCL runtime = 0.941198  
   Speedup = 11.330891  

