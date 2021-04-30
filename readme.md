Implementation of the representative scenario algorithm proposed in ``Bengio, Y., Frejinger, E., Lodi, A., Patel, R., & Sankaranarayanan, S. (2020, September). A learning-based algorithm to quickly compute good primal solutions for Stochastic Integer Programs. In International Conference on Integration of Constraint Programming, Artificial Intelligence, and Operations Research (pp. 99-111). Springer, Cham.``

This implementation has been developed by Warley Almeida Silva as part of the final project of the IFT 6512 Stochastic Programming course. The course has been taught by professor Fabian Bastin at Université de Montréal during the Winter semester of 2022. The problem considered in this implementation is the Stochastic Capacitated Facility Location Problem (SCFLP). Please find the latest version of the report [here](https://drive.google.com/file/d/1wZ386YchkVDBY9rvVx_8wORuE4IoiHkx/view?usp=sharing).


Quick explanation about the structure of this repository:
1. Inside the root folder:
- File `IFT6512 - Project.ipnyb` contains the implementation of the representative scenario algorithm;
- Folder ``instances`` contains SCFLP instance files identified by the instance number;
- Folder ``outputs`` contains solver outputs of the deterministic SCFLP identified by the instance number;
- Folder ``scenarios`` contains representative scenarios found by the heuristic identified by the instance number;
- File ``training.txt`` contains instance identifiers of the randomly selected instances to be in the training set;
- File ``regression.txt`` contains the linear regression model trained to predict the representative scenario.
2. Inside ``lambda`` and ``gamma`` folders:
- Folder ``results`` contains performance summaries of the approaches identified by the instance number;
- Folder ``detailed`` contains solver outputs of the approaches identified by the instance number and the name of the approach;
- Folder ``constrained`` contains solver outputs of the restricted SCFLP (where the first-stage decisions are fixed to the first-stage decisions given by the approaches) identified by the instance number.

**Important notes**:
- Every mention of a ``HDG`` approach actually refers to the ``APR`` approach explained in the report;
- Create folders ``results``, ``detailed``, and ``constrained`` in the root folder before executing the code.