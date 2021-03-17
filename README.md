# Adult Income Analysis
Prediction whether income exceeds $50K/yr based on census data. 

I collected the data from the UCI Machine Learning repository.

### ROC Curve of my models: 
![]data:image/png;base64,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eQzqIy8vTzQ0NIj6+nohhBBZWVneD7hf//rX4p133vFpn5mZKW688UYRExMjXC6XVzx0Pl599VXxhz/8wads3759XvHW+YPklltuEStXrvS2KywsFDNnzhSgWQV+8YtfeOsURRFNTU1e65kQQsydO7fHe/vd734n/v3vf/v0t1qtXutfXl6euOOOO7z1CxcuFAcOHOjzPdx88829Ptvt27eLn/zkJwL6Js6am5uFTqfz1peVlYnp06cLVVWF3W73igegV8vZo48+Kj799NNu69566y2xZMkSn3veu3dvj/dQXV0tJk6cKEATVGvXru31nh944AHvta+55hrxww8/dNvucHEWHR0tWltbfUT2NddcI1atWuV9fgUFBT5jdH6mc+fOFT/++KOYPn26UBSlx+fc+fe+/Xdw37593p/T8RwzZswQJSUlPmW33nqrWL16dbftn3rqKbF+/XoRGRkphgwZIjZv3iyEECImJuaIYwUEBIjc3FwxbNiwLvcjD3kM9kP6nEkkfeDSSy8lODiY2bNnM27cOCIjIwFITEzkqquuoqamxnvMmDGD2NhYEhISqK6upra2tst4iYmJPPTQQz79EhISiIuL69L2448/5txzzyU2NpZZs2YhhGDdunXecV588UXvGNXV1SiKgsVi8fYvKirq8b7i4uIoKCjwngshKCoq6rF/QUGBd459uYfDr33DDTewfft2b/ukpCTvs+wLVVVVuFwu73lzczOBgYFERUVhMBh8rtfbfSckJHDw4MEe60tLS7tco50HH3yQPXv2UFtbS01NDSEhIT73cPh1R48ezRdffEFJSQl1dXX87//+r7f9kebRmcTERAwGAyUlJd7n9/rrrxMdHd2ne169ejUvv/wyr7zyCmVlZbz++usEBQX16dp9nefixYtpaGigoaGhW7/MxsZGgoODfcqCg4NpaGjodrw//vGPbN++nezsbDZu3Mjnn3+O3W6nvLz8iGM9+eSTvPvuu+Tn5/fpHiWSwYQUZxLJUfDtt9/yz3/+k7/85S+A9mH47rvvEhYW5j0CAwN59tlnKSoqIjw8nJCQkC7jFBUV8cc//tGnX0BAAB988EGXtnV1daxYsYKrr76a6667jqVLl/qMc8cdd/iMYzab2bRpk7eNEKLH+ykuLiYxMdGnLCEhAZvN5nPeztChQ72O1X25h87XHjp0KEuWLOHee+8lIiKCsLAwdu3ahaIoR5znkaioqMDhcBAfH9/tvA+nqKiIkSNHHvV1ZsyYwSOPPMLVV1/tvee6ujrvPUDX+1i8eDH79u1j9OjRhISE8Jvf/Mbbvrd5HD5OUVERbW1tREZGeq8dEhJCUlJSj30O56WXXmLKlCmcddZZjBkzhl/96ld96tfX53XXXXcRFBREUFAQf/rTn7rU5+bmotfrGTVqlLcsJSWF3bt3dztea2sr9913H/Hx8YwcOZKqqiq2bduG2+0+4lhpaWncf//9lJSUUFJSQkJCAh9++CG//vWvj3gfEslAI8WZRHKUvPDCC1xwwQWkpKTw3nvvsWjRIubPn4+qqphMJmbPno3FYqG0tJSvv/6aV199ldDQUPR6PTNnzgRgyZIl3HnnnUybNg0As9nMhRde6GOh6cz777/PjTfeyBVXXMH777/vLX/ttdd47LHHvBFqwcHBXHnllX
