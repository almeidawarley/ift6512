Implementation of the representative scenario algorithm proposed in ``Bengio, Y., Frejinger, E., Lodi, A., Patel, R., & Sankaranarayanan, S. (2020, September). A learning-based algorithm to quickly compute good primal solutions for Stochastic Integer Programs. In International Conference on Integration of Constraint Programming, Artificial Intelligence, and Operations Research (pp. 99-111). Springer, Cham.``
This implementation has been developed by Warley Almeida Silva as part of the final project of the course IFT 6512 Stochastic Programming at Université de Montréal lectured by professor Fabian Bastin. The problem considered in this implementation is the Stochastic Capacitated Facility Location Problem (SCFLP).


Quick explanation about the structure of this repository:
- Folder ``instances`` contains SCFLP instance files identified by the instance number;
- Folder ``outputs`` contains solver outputs of the deterministic SCFLP identified by the instance number;
- Folder ``scenarios`` contains representative scenarios found by the heuristic identified by the instance number;
- Folder ``results`` contains performance summaries of the computational approaches identified by the instance number;
- Folder ``detailed`` contains solver outputs of the computational approaches identified by the instance number and the name of the approach;
- Folder ``constrained`` contains solver outputs of the restricted SCFLP (where the first-stage decisions are fixed to the first-stage decisions given by the approaches) identified by the instance number;