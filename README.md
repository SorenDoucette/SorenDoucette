import scipy
import numpy
import matplotlib
import matplotlib.pyplot as plt
import platform
import socket
your_first_name = 'Soren'
your_last_name = 'Doucette'
your_github_username = 'MilleniumFalcon'
classname = 'Foundations of Physics'
term = 'Fall_2024' # must contain no spaces
plt.plot([0,1], 'r', [1,0], 'b')
plt.text( 0.5, 0.8, '{0:s} {1:s} {2:s}'
.format(your_first_name, your_last_name, your_github_username),
horizontalalignment='center',
size = 'x-large',
bbox=dict(facecolor='purple', alpha=0.4))
plt.text( 0.5, 0.1,
'{1:s}\nscipy {2:s}\nnumpy {3:s}\nmatplotlib {4:s}\non {5:s}\n{6:s}'
.format(
classname,
term,
scipy.__version__,
numpy.__version__,
matplotlib.__version__,
platform.platform(),
socket.gethostname()
) ,
horizontalalignment='center'
)
filename = your_last_name + '_' + your_first_name + '_' + term + '.png'
plt.title('*** Turn in the saved version of this plot as Python Assignment 0 ***\
n',fontsize=12)
plt.savefig(filename)
plt.show()
#Check successful use of np
a=numpy.sqrt(2)
print(a)
