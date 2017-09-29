    import numpy as np 

    import matplotlib.pyplot as plt

    V = [0.]  
    t = [0.] 
    g = 9.8 
    dt = 0.5 
    end_time = 20

    for i in range(int(end_time / dt)):

	    tmp = V[i] - g * dt

	    V.append(tmp)

	    t.append(dt * (i + 1))     #euler 法

	    print t[-1], V[-1]

    plt.figure(figsize=(8,6)) 

    plt.plot(t,V,label="V(t)",color="red",linewidth=1)

    plt.xlabel("t(s)") 

    plt.ylabel("V(m/s)") 

    plt.legend()  

    plt.show()  
    © 2017 GitHub, Inc.
