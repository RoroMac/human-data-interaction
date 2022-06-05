{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "dying-climate",
   "metadata": {},
   "source": [
    "# A4: Final Project\n",
    "\n",
    "The final project for HCDE410 investigating the impact that collegiate sports have on their universities. This repo is protected under the MIT license."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "challenging-weather",
   "metadata": {},
   "source": [
    "I merged the NCAA college football dataset with the college scorecard dataset to determine the impact that the college football coach has on college admission. I randomly sampled 60 universities at different years and annotated these datasets with the head coach football salary at the given time. In determining if there was any relationship I ran two pearson coefficient functions between admission rates and win rates and admission rates and coach salary. Both suggest that to no significant degree that coach salary and football winnings has on a university prestige and suggests the Flutie effect to be false."
   ]
  },
  {
   "cell_type": "markdown",
   "id": "favorite-clearing",
   "metadata": {},
   "source": [
    "# A7 Final Project.ipynb\n",
    "\n",
    "This file is the primary research report. It includes methods for data cleaning, producing the data visualization, and running an analysis comparing admissions, salary, and college football win rates. It produces all datasets used in the clean data and datavisualizations folder.\n",
    "\n",
    "# Project Proposal\n",
    "\n",
    "A text file describing motivations of this project. There are no outputs or dependencies.\n",
    "\n",
    "# Raw Data\n",
    "\n",
    "Includes the datasets used in the analysis coming from the college scorecard and the NCAA college football dataset.\n",
    "\n",
    "### College Scorecard\n",
    "\n",
    "A federal database for reporting publicly available data from public institutions. Private universities do not have to report and therefore information provided by them may be missing. The scorecard dataset does not have a license but assumed as public domain. Variables of interest include\n",
    "\n",
    "| Variable | Description |\n",
    "|-|-|\n",
    "| Institution Name | Used to join college scorecard data to football dataset |\n",
    "|Admission Rate | Admission rate of the given year, used to calculate change in admission rates between two years|\n",
    "|Control | Determine a public institution|\n",
    "|UGDS | Size of an undergraduate student population |\n",
    "| HIGHDEG | The highest degree provided at the instititution|\n",
    "\n",
    "### NCAA College Football Dataset\n",
    "\n",
    "A dataset from the NCAA college football but provided under an open data license. This is used to track win ratios of certain institutions to later determine correlation with school admission rate. Variables of interest include\n",
    "\n",
    "| Variable | Description |\n",
    "|-|-|\n",
    "| Institution Name | Name of the college team |\n",
    "| Number of Games played | Number of games played for the given year\n",
    "| Number of Games Won | Number of games wno for the given year |"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "cleared-treat",
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.7.2"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
