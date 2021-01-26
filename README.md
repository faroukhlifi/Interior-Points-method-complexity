# interior_point_methods

Research projet I made with Farouk Khlifi under the supervision of professors Xavier Allamigeon and Stéphane Gaubert, Ecole polytechnique. In this repository, you will find the code we developped, as well as the abstract of our work below.

ACKNOWLEDGMENTS
Our deep gratitude goes to professor Xavier Allamigeon and to professor Stéphane Gaubert, who met with us each week to review our findings, suggest new ideas and share their thoughts with us. We thank them sincerely for their kindness and dedication.

ABSTRACT
Interior-point methods are a very important class of algorithms for linear programming. In this paper, we follow on a previous work by Xavier Allamigeon, Pascal Benchimol, Stéphane Gaubert and Michael Joswig “Log-barrier interior point methods are not strongly polynomial" ([1], https://arxiv.org/abs/1708.01544) proving that log-barrier primal-dual interior-point methods are not strongly polynomial by presenting a counter-example.  More precisely, we analyze an innovative algorithm proposed by Lee and Sidford in "Solving Linear Programs with Sqrt(rank) Linear System Solves” ([2], https://arxiv.org/abs/1910.08033), generalizing interior-point methods mainly by introducing "weighted path finding", with the objective to extend the results proven in [1] to this algorithm.
Our main finding is that a central path associated with a certain barrier-function that we determine lie in fact at the core of this algorithm. For instance, the last steps performed by the algorithm at the end for a fixed value of t converge towards a point of the central path (if it converges, which is the case in practice in this algorithm). Moreover, in an informal sense, throughout the execution of the algorithm, x remains close to this central path. We find a numerical scheme to approximate this central path, and our second important finding from numerical simulations is that the tropical central path is highly likely to be exactly the same as the one associated with the classical log-barrier. This opens the door to a proof of the non strongly polynomial complexity of this new algorithm by adapting the ideas of the proof of Allamigeon et al.


