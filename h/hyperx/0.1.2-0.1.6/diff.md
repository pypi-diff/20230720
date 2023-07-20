# Comparing `tmp/hyperx-0.1.2.tar.gz` & `tmp/hyperx-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperx-0.1.2.tar", last modified: Mon Jul 10 15:33:58 2023, max compression
+gzip compressed data, was "hyperx-0.1.6.tar", last modified: Thu Jul 20 18:49:09 2023, max compression
```

## Comparing `hyperx-0.1.2.tar` & `hyperx-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.428981 hyperx-0.1.2/
--rw-rw-rw-   0        0        0      535 2023-07-10 15:33:58.428036 hyperx-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.352293 hyperx-0.1.2/hyperx/
--rw-rw-rw-   0        0        0      747 2023-06-29 20:58:54.000000 hyperx-0.1.2/hyperx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.401576 hyperx-0.1.2/hyperx/api/
--rw-rw-rw-   0        0        0   145840 2023-07-10 15:31:55.000000 hyperx-0.1.2/hyperx/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.405943 hyperx-0.1.2/hyperx/api/types/
--rw-rw-rw-   0        0        0    24178 2023-07-10 15:31:23.000000 hyperx-0.1.2/hyperx/api/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.417962 hyperx-0.1.2/hyperx/library/
--rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.2/hyperx/library/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.2/hyperx/library/find.py
--rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.2/hyperx/library/library.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.424990 hyperx-0.1.2/hyperx/utils/
--rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.2/hyperx/utils/__init__.py
--rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.2/hyperx/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:33:58.397573 hyperx-0.1.2/hyperx.egg-info/
--rw-rw-rw-   0        0        0      535 2023-07-10 15:33:58.000000 hyperx-0.1.2/hyperx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-07-10 15:33:58.000000 hyperx-0.1.2/hyperx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 15:33:58.000000 hyperx-0.1.2/hyperx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-10 15:33:58.000000 hyperx-0.1.2/hyperx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 15:33:58.000000 hyperx-0.1.2/hyperx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      660 2023-07-10 15:30:01.000000 hyperx-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 15:33:58.429983 hyperx-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.622119 hyperx-0.1.6/
+-rw-rw-rw-   0        0        0      535 2023-07-20 18:49:09.621151 hyperx-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.580562 hyperx-0.1.6/hyperx/
+-rw-rw-rw-   0        0        0      747 2023-07-17 20:06:12.000000 hyperx-0.1.6/hyperx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.607388 hyperx-0.1.6/hyperx/api/
+-rw-rw-rw-   0        0        0   156811 2023-07-20 18:48:41.000000 hyperx-0.1.6/hyperx/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.609605 hyperx-0.1.6/hyperx/api/types/
+-rw-rw-rw-   0        0        0    23328 2023-07-20 18:48:20.000000 hyperx-0.1.6/hyperx/api/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.616165 hyperx-0.1.6/hyperx/library/
+-rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.6/hyperx/library/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.6/hyperx/library/find.py
+-rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.6/hyperx/library/library.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.620148 hyperx-0.1.6/hyperx/utils/
+-rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.6/hyperx/utils/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.6/hyperx/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:49:09.605386 hyperx-0.1.6/hyperx.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-07-20 18:49:09.000000 hyperx-0.1.6/hyperx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-07-20 18:49:09.000000 hyperx-0.1.6/hyperx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 18:49:09.000000 hyperx-0.1.6/hyperx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-20 18:49:09.000000 hyperx-0.1.6/hyperx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 18:49:09.000000 hyperx-0.1.6/hyperx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      660 2023-07-20 18:39:47.000000 hyperx-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 18:49:09.622897 hyperx-0.1.6/setup.cfg
```

### Comparing `hyperx-0.1.2/PKG-INFO` & `hyperx-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.2
+Version: 0.1.6
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.2/hyperx/__init__.py` & `hyperx-0.1.6/hyperx/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.2/hyperx/api/__init__.py` & `hyperx-0.1.6/hyperx/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ..library import _api, _types
 
 from ..api import types
 from typing import TypeVar, Generic, overload
 from enum import Enum
-from System.Collections.Generic import List, IEnumerable
+from System.Collections.Generic import List, IEnumerable, Dictionary
 from System.Threading.Tasks import Task
 from System import Guid, DateTime
 
 from abc import ABC, abstractmethod
 
 T = TypeVar('T')
 
@@ -17,31 +17,41 @@
 		for thing in ints:
 			if thing is not None:
 				intsList.Add(thing)
 	
 	return intsList
 
 class AnalysisResultToReturn(Enum):
+	'''
+	Used to specify which analysis result to return.
+	'''
 	Limit = 1
 	Ultimate = 2
 	Minimum = 3
 
 class CollectionModificationStatus(Enum):
+	'''
+	Indicates that whether a collection was manipulated successfully.
+	'''
 	Success = 1
 	DuplicateIdFailure = 2
 	EntityMissingAddFailure = 3
 	EntityMissingRemovalFailure = 4
 	FemConnectionFailure = 5
 
 class CreateDatabaseStatus(Enum):
 	Success = 1
 	TemplateNotFound = 2
 	ImproperExtension = 3
 
 class MaterialCreationStatus(Enum):
+	'''
+	Indicates that whether a Material was created successfully. 
+            If not, this indicates why the material was not created.
+	'''
 	Success = 1
 	DuplicateNameFailure = 2
 	DuplicateFemIdFailure = 3
 	MissingMaterialToCopy = 4
 
 class DbForceUnit(Enum):
 	Pounds = 1
@@ -65,19 +75,27 @@
 class DbTemperatureUnit(Enum):
 	Fahrenheit = 1
 	Rankine = 2
 	Celsius = 3
 	Kelvin = 4
 
 class ProjectCreationStatus(Enum):
+	'''
+	Indicates that whether a Material was created successfully. 
+            If not, this indicates why the material was not created.
+	'''
 	Success = 1
 	Failure = 2
 	DuplicateNameFailure = 3
 
 class ProjectDeletionStatus(Enum):
+	'''
+	Indicates that whether a Material was created successfully. 
+            If not, this indicates why the material was not created.
+	'''
 	Success = 1
 	Failure = 2
 	ProjectDoesNotExistFailure = 3
 	ActiveProjectFailure = 4
 
 class SetUnitsStatus(Enum):
 	Success = 1
@@ -114,28 +132,37 @@
 	RundeckCommitFailure = 7
 
 class ZoneIdUpdateStatus(Enum):
 	Success = 1
 	DuplicateIdFailure = 2
 
 class UnitSystem(Enum):
+	'''
+	Unit system specified when starting a scripting Application.
+	'''
 	English = 1
 	SI = 2
 
 
 class IdEntity(ABC):
+	'''
+	Represents an entity with an ID.
+	'''
 	def __init__(self, idEntity: _api.IdEntity):
 		self._Entity = idEntity
 
 	@property
 	def Id(self) -> int:
 		return self._Entity.Id
 
 
 class IdNameEntity(IdEntity):
+	'''
+	Represents an entity with an ID and Name.
+	'''
 	def __init__(self, idNameEntity: _api.IdNameEntity):
 		self._Entity = idNameEntity
 
 	@property
 	def Name(self) -> str:
 		return self._Entity.Name
 
@@ -149,14 +176,17 @@
 
 	@property
 	def Description(self) -> str:
 		return self._Entity.Description
 
 
 class Margin:
+	'''
+	Represents a Margin result.
+	'''
 	def __init__(self, margin: _api.Margin):
 		self._Entity = margin
 
 	@property
 	def AdjustedMargin(self) -> float:
 		return self._Entity.AdjustedMargin
 
@@ -170,93 +200,120 @@
 
 	@property
 	def MarginCode(self) -> types.MarginCode:
 		return types.MarginCode[self._Entity.MarginCode.ToString()]
 
 
 class AnalysisResult(ABC):
+	'''
+	Contains result information for an analysis
+	'''
 	def __init__(self, analysisResult: _api.AnalysisResult):
 		self._Entity = analysisResult
 
 	@property
 	def LimitUltimate(self) -> types.LimitUltimate:
+		'''
+		Limit vs Ultimate loads.
+		'''
 		return types.LimitUltimate[self._Entity.LimitUltimate.ToString()]
 
 	@property
 	def LoadCaseId(self) -> int:
 		return self._Entity.LoadCaseId
 
 	@property
 	def Margin(self) -> Margin:
+		'''
+		Represents a Margin result.
+		'''
 		return Margin(self._Entity.Margin)
 
 	@property
 	def AnalysisDefinition(self) -> AnalysisDefinition:
 		return AnalysisDefinition(self._Entity.AnalysisDefinition)
 
 
 class JointAnalysisResult(AnalysisResult):
 	def __init__(self, jointAnalysisResult: _api.JointAnalysisResult):
 		self._Entity = jointAnalysisResult
 
 	@property
 	def ObjectId(self) -> types.JointObject:
+		'''
+		Enum identifying the possible entities within a joint
+		'''
 		return types.JointObject[self._Entity.ObjectId.ToString()]
 
 
 class ZoneAnalysisConceptResult(AnalysisResult):
 	def __init__(self, zoneAnalysisConceptResult: _api.ZoneAnalysisConceptResult):
 		self._Entity = zoneAnalysisConceptResult
 
 	@property
 	def ConceptId(self) -> types.FamilyConceptUID:
+		'''
+		Values match UID of family_concept_definition table.
+		'''
 		return types.FamilyConceptUID[self._Entity.ConceptId.ToString()]
 
 
 class ZoneAnalysisObjectResult(AnalysisResult):
 	def __init__(self, zoneAnalysisObjectResult: _api.ZoneAnalysisObjectResult):
 		self._Entity = zoneAnalysisObjectResult
 
 	@property
 	def ObjectId(self) -> types.FamilyObjectUID:
+		'''
+		Values match UID of family_object_definition table.
+		'''
 		return types.FamilyObjectUID[self._Entity.ObjectId.ToString()]
 
 
 class AssignableProperty(IdNameEntity):
 	def __init__(self, assignableProperty: _api.AssignableProperty):
 		self._Entity = assignableProperty
 
 
 class AssignablePropertyWithFamilyCategory(AssignableProperty):
 	def __init__(self, assignablePropertyWithFamilyCategory: _api.AssignablePropertyWithFamilyCategory):
 		self._Entity = assignablePropertyWithFamilyCategory
 
 	@property
 	def FamilyCategory(self) -> types.FamilyCategory:
+		'''
+		Representative of the family_category table
+		'''
 		return types.FamilyCategory[self._Entity.FamilyCategory.ToString()]
 
 
 class FailureObjectGroup(IdNameEntity):
 	def __init__(self, failureObjectGroup: _api.FailureObjectGroup):
 		self._Entity = failureObjectGroup
 
 	@property
 	def IsEnabled(self) -> bool:
 		return self._Entity.IsEnabled
 
 	@property
 	def LimitUltimate(self) -> types.LimitUltimate:
+		'''
+		Limit vs Ultimate loads.
+		'''
 		return types.LimitUltimate[self._Entity.LimitUltimate.ToString()]
 
 	@property
 	def RequiredMargin(self) -> float:
 		return self._Entity.RequiredMargin
 
 
 class FailureSetting(IdNameEntity):
+	'''
+	Setting for a Failure Mode or a Failure Criteria.
+	'''
 	def __init__(self, failureSetting: _api.FailureSetting):
 		self._Entity = failureSetting
 
 	@property
 	def CategoryId(self) -> int:
 		return self._Entity.CategoryId
 
@@ -301,14 +358,18 @@
 	def __init__(self, idEntityCol: _api.IdEntityCol):
 		self._Entity = idEntityCol
 
 	@property
 	def IdEntityColList(self) -> tuple[IdEntity]:
 		return tuple([IdEntity(idEntityCol) for idEntityCol in self._Entity])
 
+	@property
+	def Ids(self) -> tuple[int]:
+		return tuple([int(int32) for int32 in self._Entity.Ids])
+
 	def Contains(self, id: int) -> bool:
 		return self._Entity.Contains(id)
 
 	def Count(self) -> int:
 		return self._Entity.Count()
 
 	def Get(self, id: int) -> T:
@@ -329,26 +390,30 @@
 		self._Entity = idNameEntityCol
 		self._CollectedClass = T
 
 	@property
 	def IdNameEntityColList(self) -> tuple[T]:
 		return tuple([T(idNameEntityCol) for idNameEntityCol in self._Entity])
 
+	@property
+	def Names(self) -> tuple[str]:
+		return tuple([str(string) for string in self._Entity.Names])
+
 	@overload
 	def Get(self, name: str) -> T: ...
 
 	@overload
 	def Get(self, id: int) -> T: ...
 
 	def Get(self, item1 = None) -> T:
 		if isinstance(item1, str):
 			return self._Entity.Get(item1)
 
 		if isinstance(item1, int):
-			return T(super().Get(item1))
+			return super().Get(item1)
 
 		return self._Entity.Get(item1)
 
 	def __getitem__(self, index: int):
 		return self.IdNameEntityColList[index]
 
 	def __iter__(self):
@@ -696,14 +761,17 @@
 
 	@property
 	def Subcase(self) -> DesignLoadSubcase:
 		return DesignLoadSubcase(self._Entity.Subcase)
 
 	@property
 	def TemperatureChoiceType(self) -> types.TemperatureChoiceType:
+		'''
+		Load Case Setting selection for analysis and initial temperature.
+		'''
 		return types.TemperatureChoiceType[self._Entity.TemperatureChoiceType.ToString()]
 
 	@property
 	def Value(self) -> float:
 		return self._Entity.Value
 
 
@@ -783,14 +851,17 @@
 
 	@property
 	def UID(self) -> Guid:
 		return self._Entity.UID
 
 
 class Vector3d:
+	'''
+	Represents a readonly 3D vector.
+	'''
 	def __init__(self, vector3d: _api.Vector3d):
 		self._Entity = vector3d
 
 	@property
 	def X(self) -> float:
 		return self._Entity.X
 
@@ -820,17 +891,20 @@
 	def __eq__(self, other):
 		return self.Equals(other)
 
 	def __ne__(self, other):
 		return not self.Equals(other)
 
 
-class DiscreteFieldTable(IdNameEntityRenameable):
-	def __init__(self, discreteFieldTable: _api.DiscreteFieldTable):
-		self._Entity = discreteFieldTable
+class DiscreteField(IdNameEntityRenameable):
+	'''
+	Represents a table of discrete field data.
+	'''
+	def __init__(self, discreteField: _api.DiscreteField):
+		self._Entity = discreteField
 
 	@property
 	def Columns(self) -> dict[int, str]:
 		columnsDict = {}
 		for kvp in self._Entity.Columns:
 			columnsDict[int(kvp.Key)] = str(kvp.Value)
 
@@ -838,18 +912,24 @@
 
 	@property
 	def ColumnCount(self) -> int:
 		return self._Entity.ColumnCount
 
 	@property
 	def DataType(self) -> types.DiscreteFieldDataType:
+		'''
+		Defines the type of data stored in a Discrete Field. Such as Vector, Scalar, String.
+		'''
 		return types.DiscreteFieldDataType[self._Entity.DataType.ToString()]
 
 	@property
 	def PhysicalEntityType(self) -> types.DiscreteFieldPhysicalEntityType:
+		'''
+		Defines the type of physical entity that a Discrete Field applies to, such as zone, element, joint, etc.
+		'''
 		return types.DiscreteFieldPhysicalEntityType[self._Entity.PhysicalEntityType.ToString()]
 
 	@property
 	def PointIds(self) -> list[Vector3d]:
 		return [Vector3d(vector3d) for vector3d in self._Entity.PointIds]
 
 	@property
@@ -890,26 +970,32 @@
 	@overload
 	def SetStringValue(self, entityId: int, columnId: int, value: str) -> None: ...
 
 	@overload
 	def SetStringValue(self, pointId: Vector3d, columnId: int, value: str) -> None: ...
 
 	def DeleteAllRows(self) -> None:
+		'''
+		Delete all rows for this discrete field.
+		'''
 		return self._Entity.DeleteAllRows()
 
 	def DeleteColumn(self, columnId: int) -> None:
 		return self._Entity.DeleteColumn(columnId)
 
 	def DeletePointRow(self, pointId: Vector3d) -> None:
 		return self._Entity.DeletePointRow(pointId._Entity)
 
 	def DeleteRow(self, entityId: int) -> None:
 		return self._Entity.DeleteRow(entityId)
 
 	def DeleteRowsAndColumns(self) -> None:
+		'''
+		Delete all rows and columns for this discrete field.
+		'''
 		return self._Entity.DeleteRowsAndColumns()
 
 	def ReadNumericCell(self, item1 = None, item2 = None) -> float:
 		if isinstance(item1, int) and isinstance(item2, int):
 			return self._Entity.ReadNumericCell(item1, item2)
 
 		if isinstance(item1, Vector3d) and isinstance(item2, int):
@@ -1036,14 +1122,17 @@
 		yield from self.AnalysisResultColList
 
 	def __len__(self):
 		return len(self.AnalysisResultColList)
 
 
 class ZoneJointEntity(EntityWithAssignableProperties):
+	'''
+	Abstract base for a Zone or Joint.
+	'''
 	def __init__(self, zoneJointEntity: _api.ZoneJointEntity):
 		self._Entity = zoneJointEntity
 
 	@abstractmethod
 	def GetMinimumMargin(self) -> Margin:
 		return Margin(self._Entity.GetMinimumMargin())
 
@@ -1067,14 +1156,17 @@
 		return AnalysisResult(self._Entity.GetControllingResult())
 
 	def GetMinimumMargin(self) -> Margin:
 		return Margin(self._Entity.GetMinimumMargin())
 
 
 class ZoneBase(ZoneJointEntity):
+	'''
+	Abstract for regular Zones and Panel Segments.
+	'''
 	def __init__(self, zoneBase: _api.ZoneBase):
 		self._Entity = zoneBase
 
 	@property
 	def Centroid(self) -> Centroid:
 		return Centroid(self._Entity.Centroid)
 
@@ -1156,14 +1248,17 @@
 	def SetObjectElements(self, discreteDefinitionType: types.DiscreteDefinitionType, elementIds: tuple[int]) -> None:
 		elementIdsList = MakeCSharpIntList(elementIds)
 		elementIdsEnumerable = IEnumerable(elementIdsList)
 		return self._Entity.SetObjectElements(_types.DiscreteDefinitionType(discreteDefinitionType.value), elementIdsEnumerable)
 
 
 class Zone(ZoneBase):
+	'''
+	Abstract for regular Zones (not Panel Segments).
+	'''
 	def __init__(self, zone: _api.Zone):
 		self._Entity = zone
 
 	@property
 	def Elements(self) -> ElementCol:
 		return ElementCol(self._Entity.Elements)
 
@@ -1189,18 +1284,18 @@
 	def Get(self, name: str) -> T: ...
 
 	@overload
 	def Get(self, id: int) -> T: ...
 
 	def Get(self, item1 = None) -> T:
 		if isinstance(item1, str):
-			return T(super().Get(item1))
+			return super().Get(item1)
 
 		if isinstance(item1, int):
-			return T(super().Get(item1))
+			return super().Get(item1)
 
 		return self._Entity.Get(item1)
 
 	def __getitem__(self, index: int):
 		return self.EntityWithAssignablePropertiesColList[index]
 
 	def __iter__(self):
@@ -1309,14 +1404,17 @@
 		yield from self.ZoneColList
 
 	def __len__(self):
 		return len(self.ZoneColList)
 
 
 class ZoneJointContainer(IdNameEntityRenameable):
+	'''
+	Represents an entity that contains a collection of Zones and Joints.
+	'''
 	def __init__(self, zoneJointContainer: _api.ZoneJointContainer):
 		self._Entity = zoneJointContainer
 
 	@property
 	def Centroid(self) -> Centroid:
 		return Centroid(self._Entity.Centroid)
 
@@ -1483,14 +1581,17 @@
 		if isinstance(item1, PanelSegmentCol):
 			return CollectionModificationStatus[self._Entity.RemovePanelSegments(item1._Entity).ToString()]
 
 		return self._Entity.RemovePanelSegments(segmentIdsEnumerable)
 
 
 class FoamTemperature:
+	'''
+	Foam material temperature dependent properties.
+	'''
 	def __init__(self, foamTemperature: _api.FoamTemperature):
 		self._Entity = foamTemperature
 
 	@property
 	def Temperature(self) -> float:
 		return self._Entity.Temperature
 
@@ -1576,14 +1677,17 @@
 
 	@C.setter
 	def C(self, value: float) -> None:
 		self._Entity.C = value
 
 
 class Foam:
+	'''
+	Foam material.
+	'''
 	def __init__(self, foam: _api.Foam):
 		self._Entity = foam
 
 	@property
 	def MaterialFamilyName(self) -> str:
 		return self._Entity.MaterialFamilyName
 
@@ -1639,14 +1743,18 @@
 	def Absorption(self) -> float:
 		return self._Entity.Absorption
 
 	@property
 	def Manufacturer(self) -> str:
 		return self._Entity.Manufacturer
 
+	@property
+	def FoamTemperatureProperties(self) -> list[FoamTemperature]:
+		return [FoamTemperature(foamTemperature) for foamTemperature in self._Entity.FoamTemperatureProperties]
+
 	@MaterialFamilyName.setter
 	def MaterialFamilyName(self, value: str) -> None:
 		self._Entity.MaterialFamilyName = value
 
 	@Name.setter
 	def Name(self, value: str) -> None:
 		self._Entity.Name = value
@@ -1701,18 +1809,24 @@
 	def DeleteTemperatureProperty(self, temperature: float) -> bool:
 		return self._Entity.DeleteTemperatureProperty(temperature)
 
 	def GetTemperature(self, lookupTemperature: float) -> FoamTemperature:
 		return FoamTemperature(self._Entity.GetTemperature(lookupTemperature))
 
 	def Save(self) -> None:
+		'''
+		Save any changes to this foam material to the database.
+		'''
 		return self._Entity.Save()
 
 
 class HoneycombTemperature:
+	'''
+	Honeycomb material temperature dependent properties.
+	'''
 	def __init__(self, honeycombTemperature: _api.HoneycombTemperature):
 		self._Entity = honeycombTemperature
 
 	@property
 	def Temperature(self) -> float:
 		return self._Entity.Temperature
 
@@ -1846,14 +1960,17 @@
 
 	@C.setter
 	def C(self, value: float) -> None:
 		self._Entity.C = value
 
 
 class Honeycomb:
+	'''
+	Honeycomb material.
+	'''
 	def __init__(self, honeycomb: _api.Honeycomb):
 		self._Entity = honeycomb
 
 	@property
 	def MaterialFamilyName(self) -> str:
 		return self._Entity.MaterialFamilyName
 
@@ -1905,14 +2022,18 @@
 	def CellSize(self) -> float:
 		return self._Entity.CellSize
 
 	@property
 	def Manufacturer(self) -> str:
 		return self._Entity.Manufacturer
 
+	@property
+	def HoneycombTemperatureProperties(self) -> list[HoneycombTemperature]:
+		return [HoneycombTemperature(honeycombTemperature) for honeycombTemperature in self._Entity.HoneycombTemperatureProperties]
+
 	@MaterialFamilyName.setter
 	def MaterialFamilyName(self, value: str) -> None:
 		self._Entity.MaterialFamilyName = value
 
 	@Name.setter
 	def Name(self, value: str) -> None:
 		self._Entity.Name = value
@@ -1963,18 +2084,24 @@
 	def DeleteTemperatureProperty(self, temperature: float) -> bool:
 		return self._Entity.DeleteTemperatureProperty(temperature)
 
 	def GetTemperature(self, lookupTemperature: float) -> HoneycombTemperature:
 		return HoneycombTemperature(self._Entity.GetTemperature(lookupTemperature))
 
 	def Save(self) -> None:
+		'''
+		Save any changes to this honeycomb material to the database.
+		'''
 		return self._Entity.Save()
 
 
 class IsotropicTemperature:
+	'''
+	Isotropic material temperature dependent properties.
+	'''
 	def __init__(self, isotropicTemperature: _api.IsotropicTemperature):
 		self._Entity = isotropicTemperature
 
 	@property
 	def Temperature(self) -> float:
 		return self._Entity.Temperature
 
@@ -2244,14 +2371,17 @@
 
 	@FcFatigue.setter
 	def FcFatigue(self, value: float) -> None:
 		self._Entity.FcFatigue = value
 
 
 class Isotropic:
+	'''
+	Isotropic material.
+	'''
 	def __init__(self, isotropic: _api.Isotropic):
 		self._Entity = isotropic
 
 	@property
 	def MaterialFamilyName(self) -> str:
 		return self._Entity.MaterialFamilyName
 
@@ -2303,14 +2433,18 @@
 	def Cost(self) -> float:
 		return self._Entity.Cost
 
 	@property
 	def BucklingStiffnessKnockdown(self) -> float:
 		return self._Entity.BucklingStiffnessKnockdown
 
+	@property
+	def IsotropicTemperatureProperties(self) -> list[IsotropicTemperature]:
+		return [IsotropicTemperature(isotropicTemperature) for isotropicTemperature in self._Entity.IsotropicTemperatureProperties]
+
 	@MaterialFamilyName.setter
 	def MaterialFamilyName(self, value: str) -> None:
 		self._Entity.MaterialFamilyName = value
 
 	@Name.setter
 	def Name(self, value: str) -> None:
 		self._Entity.Name = value
@@ -2361,81 +2495,159 @@
 	def DeleteTemperatureProperty(self, temperature: float) -> bool:
 		return self._Entity.DeleteTemperatureProperty(temperature)
 
 	def GetTemperature(self, lookupTemperature: float) -> IsotropicTemperature:
 		return IsotropicTemperature(self._Entity.GetTemperature(lookupTemperature))
 
 	def Save(self) -> None:
+		'''
+		Save any changes to this isotropic material to the database.
+		'''
 		return self._Entity.Save()
 
 
 class OrthotropicCorrectionFactorBase(ABC):
+	'''
+	Orthotropic material correction factor.
+	'''
 	def __init__(self, orthotropicCorrectionFactorBase: _api.OrthotropicCorrectionFactorBase):
 		self._Entity = orthotropicCorrectionFactorBase
 
 	@property
 	def CorrectionId(self) -> types.CorrectionId:
+		'''
+		Correction ID for a correction factor. (Columns in HyperX)
+		'''
 		return types.CorrectionId[self._Entity.CorrectionId.ToString()]
 
 	@property
 	def PropertyId(self) -> types.CorrectionProperty:
+		'''
+		Property name for a correction factor. (Rows in HyperX)
+		'''
 		return types.CorrectionProperty[self._Entity.PropertyId.ToString()]
 
 
 class OrthotropicCorrectionFactorValue:
+	'''
+	Orthotropic material correction factor value.
+	'''
 	def __init__(self, orthotropicCorrectionFactorValue: _api.OrthotropicCorrectionFactorValue):
 		self._Entity = orthotropicCorrectionFactorValue
 
 	@property
 	def Property(self) -> types.CorrectionProperty:
+		'''
+		Property name for a correction factor. (Rows in HyperX)
+		'''
 		return types.CorrectionProperty[self._Entity.Property.ToString()]
 
 	@property
 	def Correction(self) -> types.CorrectionId:
+		'''
+		Correction ID for a correction factor. (Columns in HyperX)
+		'''
 		return types.CorrectionId[self._Entity.Correction.ToString()]
 
 	@property
 	def Equation(self) -> types.CorrectionEquation:
+		'''
+		Equation for a correction factor.
+		'''
 		return types.CorrectionEquation[self._Entity.Equation.ToString()]
 
 	@property
 	def EquationParameter(self) -> types.EquationParameterId:
+		'''
+		Correction factor parameter names.
+		'''
 		return types.EquationParameterId[self._Entity.EquationParameter.ToString()]
 
 	@property
 	def Value(self) -> float:
 		return self._Entity.Value
 
 	@Value.setter
 	def Value(self, value: float) -> None:
 		self._Entity.Value = value
 
 
 class OrthotropicEquationCorrectionFactor(OrthotropicCorrectionFactorBase):
+	'''
+	Represents an equation-based orthotropic material correction factor.
+	'''
 	def __init__(self, orthotropicEquationCorrectionFactor: _api.OrthotropicEquationCorrectionFactor):
 		self._Entity = orthotropicEquationCorrectionFactor
 
 	@property
 	def Equation(self) -> types.CorrectionEquation:
+		'''
+		Equation for a correction factor.
+		'''
 		return types.CorrectionEquation[self._Entity.Equation.ToString()]
 
+	@property
+	def OrthotropicCorrectionValues(self) -> dict[types.EquationParameterId, OrthotropicCorrectionFactorValue]:
+		orthotropicCorrectionValuesDict = {}
+		for kvp in self._Entity.OrthotropicCorrectionValues:
+			orthotropicCorrectionValuesDict[types.EquationParameterId[kvp.Key.ToString()]] = OrthotropicCorrectionFactorValue(kvp.Value)
+
+		return orthotropicCorrectionValuesDict
+
 	def AddCorrectionFactorValue(self, equationParameterName: types.EquationParameterId, valueToAdd: float) -> OrthotropicCorrectionFactorValue:
 		return OrthotropicCorrectionFactorValue(self._Entity.AddCorrectionFactorValue(_types.EquationParameterId(equationParameterName.value), valueToAdd))
 
 
+class TabularCorrectionFactorIndependentValue:
+	'''
+	Contains an independent value for a tabular correction factor row.
+	'''
+	def __init__(self, tabularCorrectionFactorIndependentValue: _api.TabularCorrectionFactorIndependentValue):
+		self._Entity = tabularCorrectionFactorIndependentValue
+
+	@property
+	def BoolValue(self) -> bool:
+		return self._Entity.BoolValue
+
+	@property
+	def DoubleValue(self) -> float:
+		return self._Entity.DoubleValue
+
+	@property
+	def IntValue(self) -> int:
+		return self._Entity.IntValue
+
+	@property
+	def ValueType(self) -> types.CorrectionValueType:
+		'''
+		Defines the type of the independent values on a tabular correction factor row.
+		'''
+		return types.CorrectionValueType[self._Entity.ValueType.ToString()]
+
+
 class TabularCorrectionFactorRow:
+	'''
+	Row data for a tabular correction factor.
+	'''
 	def __init__(self, tabularCorrectionFactorRow: _api.TabularCorrectionFactorRow):
 		self._Entity = tabularCorrectionFactorRow
 
 	@property
 	def DependentValue(self) -> float:
 		return self._Entity.DependentValue
 
+	@property
+	def IndependentValues(self) -> dict[types.CorrectionIndependentDefinition, TabularCorrectionFactorIndependentValue]:
+		return dict[types.CorrectionIndependentDefinition, TabularCorrectionFactorIndependentValue](self._Entity.IndependentValues)
+
 
 class OrthotropicTabularCorrectionFactor(OrthotropicCorrectionFactorBase):
+	'''
+	Tabular correction factor.
+	'''
 	def __init__(self, orthotropicTabularCorrectionFactor: _api.OrthotropicTabularCorrectionFactor):
 		self._Entity = orthotropicTabularCorrectionFactor
 
 	@property
 	def CorrectionFactorRows(self) -> dict[int, TabularCorrectionFactorRow]:
 		correctionFactorRowsDict = {}
 		for kvp in self._Entity.CorrectionFactorRows:
@@ -2469,19 +2681,25 @@
 		if isinstance(item1, int) and isinstance(item2, types.CorrectionIndependentDefinition) and isinstance(item3, int):
 			return self._Entity.SetIndependentValue(item1, item2, item3)
 
 		return self._Entity.SetIndependentValue(item1, item2, item3)
 
 
 class OrthotropicAllowableCurvePoint:
+	'''
+	Represents a point on a laminate allowable curve.
+	'''
 	def __init__(self, orthotropicAllowableCurvePoint: _api.OrthotropicAllowableCurvePoint):
 		self._Entity = orthotropicAllowableCurvePoint
 
 	@property
 	def Property_ID(self) -> types.AllowablePropertyName:
+		'''
+		Property name for a laminate allowable.
+		'''
 		return types.AllowablePropertyName[self._Entity.Property_ID.ToString()]
 
 	@property
 	def Temperature(self) -> float:
 		return self._Entity.Temperature
 
 	@property
@@ -2505,36 +2723,97 @@
 		self._Entity.X = value
 
 	@Y.setter
 	def Y(self, value: float) -> None:
 		self._Entity.Y = value
 
 
+class OrthotropicEffectiveLaminate:
+	'''
+	Orthotropic material effective laminate properties. Read-only from the API.
+            Check if material is an effective laminate with orthotropic.IsEffectiveLaminate.
+	'''
+	def __init__(self, orthotropicEffectiveLaminate: _api.OrthotropicEffectiveLaminate):
+		self._Entity = orthotropicEffectiveLaminate
+
+	@property
+	def Percent_tape_0(self) -> float:
+		return self._Entity.Percent_tape_0
+
+	@property
+	def Percent_tape_90(self) -> float:
+		return self._Entity.Percent_tape_90
+
+	@property
+	def Percent_tape_45(self) -> float:
+		return self._Entity.Percent_tape_45
+
+	@property
+	def Percent_fabric_0(self) -> float:
+		return self._Entity.Percent_fabric_0
+
+	@property
+	def Percent_fabric_90(self) -> float:
+		return self._Entity.Percent_fabric_90
+
+	@property
+	def Percent_fabric_45(self) -> float:
+		return self._Entity.Percent_fabric_45
+
+	@property
+	def Tape_Orthotropic(self) -> str:
+		return self._Entity.Tape_Orthotropic
+
+	@property
+	def Fabric_Orthotropic(self) -> str:
+		return self._Entity.Fabric_Orthotropic
+
+	@property
+	def Valid(self) -> bool:
+		return self._Entity.Valid
+
+	@property
+	def Use_tape_allowables(self) -> bool:
+		return self._Entity.Use_tape_allowables
+
+
 class OrthotropicLaminateAllowable:
+	'''
+	Orthotropic material laminate allowable properties.
+	'''
 	def __init__(self, orthotropicLaminateAllowable: _api.OrthotropicLaminateAllowable):
 		self._Entity = orthotropicLaminateAllowable
 
 	@property
 	def Property_ID(self) -> types.AllowablePropertyName:
+		'''
+		Property name for a laminate allowable.
+		'''
 		return types.AllowablePropertyName[self._Entity.Property_ID.ToString()]
 
 	@property
 	def Method_ID(self) -> types.AllowableMethodName:
+		'''
+		Method name for a laminate allowable.
+		'''
 		return types.AllowableMethodName[self._Entity.Method_ID.ToString()]
 
 	@Property_ID.setter
 	def Property_ID(self, value: types.AllowablePropertyName) -> None:
 		self._Entity.Property_ID = _types.AllowablePropertyName(value.value)
 
 	@Method_ID.setter
 	def Method_ID(self, value: types.AllowableMethodName) -> None:
 		self._Entity.Method_ID = _types.AllowableMethodName(value.value)
 
 
 class OrthotropicTemperature:
+	'''
+	Orthotropic material temperature dependent properties.
+	'''
 	def __init__(self, orthotropicTemperature: _api.OrthotropicTemperature):
 		self._Entity = orthotropicTemperature
 
 	@property
 	def Temperature(self) -> float:
 		return self._Entity.Temperature
 
@@ -2686,14 +2965,18 @@
 	def TTt(self) -> float:
 		return self._Entity.TTt
 
 	@property
 	def TTc(self) -> float:
 		return self._Entity.TTc
 
+	@property
+	def OrthotropicAllowableCurvePoints(self) -> list[OrthotropicAllowableCurvePoint]:
+		return [OrthotropicAllowableCurvePoint(orthotropicAllowableCurvePoint) for orthotropicAllowableCurvePoint in self._Entity.OrthotropicAllowableCurvePoints]
+
 	@Temperature.setter
 	def Temperature(self, value: float) -> None:
 		self._Entity.Temperature = value
 
 	@Et1.setter
 	def Et1(self, value: float) -> None:
 		self._Entity.Et1 = value
@@ -2853,14 +3136,17 @@
 		return self._Entity.DeleteCurvePoint(_types.AllowablePropertyName(property.value), x)
 
 	def GetCurvePoint(self, property: types.AllowablePropertyName, x: float) -> OrthotropicAllowableCurvePoint:
 		return OrthotropicAllowableCurvePoint(self._Entity.GetCurvePoint(_types.AllowablePropertyName(property.value), x))
 
 
 class Orthotropic:
+	'''
+	Orthotropic material.
+	'''
 	def __init__(self, orthotropic: _api.Orthotropic):
 		self._Entity = orthotropic
 
 	@property
 	def MaterialFamilyName(self) -> str:
 		return self._Entity.MaterialFamilyName
 
@@ -2936,14 +3222,46 @@
 	def Cost(self) -> float:
 		return self._Entity.Cost
 
 	@property
 	def BucklingStiffnessKnockdown(self) -> float:
 		return self._Entity.BucklingStiffnessKnockdown
 
+	@property
+	def OrthotropicTemperatureProperties(self) -> list[OrthotropicTemperature]:
+		return [OrthotropicTemperature(orthotropicTemperature) for orthotropicTemperature in self._Entity.OrthotropicTemperatureProperties]
+
+	@property
+	def OrthotropicLaminateAllowables(self) -> list[OrthotropicLaminateAllowable]:
+		return [OrthotropicLaminateAllowable(orthotropicLaminateAllowable) for orthotropicLaminateAllowable in self._Entity.OrthotropicLaminateAllowables]
+
+	@property
+	def OrthotropicEffectiveLaminate(self) -> OrthotropicEffectiveLaminate:
+		'''
+		Orthotropic material effective laminate properties. Read-only from the API.
+            Check if material is an effective laminate with orthotropic.IsEffectiveLaminate.
+		'''
+		return OrthotropicEffectiveLaminate(self._Entity.OrthotropicEffectiveLaminate)
+
+	@property
+	def OrthotropicEquationCorrectionFactors(self) -> dict[tuple[types.CorrectionProperty, types.CorrectionId], OrthotropicEquationCorrectionFactor]:
+		orthotropicEquationCorrectionFactorsDict = {}
+		for kvp in self._Entity.OrthotropicEquationCorrectionFactors:
+			orthotropicEquationCorrectionFactorsDict[tuple[types.CorrectionProperty, types.CorrectionId](kvp.Key)] = OrthotropicEquationCorrectionFactor(kvp.Value)
+
+		return orthotropicEquationCorrectionFactorsDict
+
+	@property
+	def OrthotropicTabularCorrectionFactors(self) -> dict[tuple[types.CorrectionProperty, types.CorrectionId], OrthotropicTabularCorrectionFactor]:
+		orthotropicTabularCorrectionFactorsDict = {}
+		for kvp in self._Entity.OrthotropicTabularCorrectionFactors:
+			orthotropicTabularCorrectionFactorsDict[tuple[types.CorrectionProperty, types.CorrectionId](kvp.Key)] = OrthotropicTabularCorrectionFactor(kvp.Value)
+
+		return orthotropicTabularCorrectionFactorsDict
+
 	@MaterialFamilyName.setter
 	def MaterialFamilyName(self, value: str) -> None:
 		self._Entity.MaterialFamilyName = value
 
 	@Name.setter
 	def Name(self, value: str) -> None:
 		self._Entity.Name = value
@@ -3018,14 +3336,17 @@
 	def DeleteTemperatureProperty(self, temperature: float) -> bool:
 		return self._Entity.DeleteTemperatureProperty(temperature)
 
 	def GetTemperature(self, lookupTemperature: float) -> OrthotropicTemperature:
 		return OrthotropicTemperature(self._Entity.GetTemperature(lookupTemperature))
 
 	def IsEffectiveLaminate(self) -> bool:
+		'''
+		Returns true if this material is an effective laminate.
+		'''
 		return self._Entity.IsEffectiveLaminate()
 
 	def HasLaminateAllowable(self, property: types.AllowablePropertyName) -> bool:
 		return self._Entity.HasLaminateAllowable(_types.AllowablePropertyName(property.value))
 
 	def AddLaminateAllowable(self, property: types.AllowablePropertyName, method: types.AllowableMethodName) -> OrthotropicLaminateAllowable:
 		return OrthotropicLaminateAllowable(self._Entity.AddLaminateAllowable(_types.AllowablePropertyName(property.value), _types.AllowableMethodName(method.value)))
@@ -3039,18 +3360,24 @@
 	def GetEquationCorrectionFactor(self, property: types.CorrectionProperty, correction: types.CorrectionId) -> OrthotropicEquationCorrectionFactor:
 		return OrthotropicEquationCorrectionFactor(self._Entity.GetEquationCorrectionFactor(_types.CorrectionProperty(property.value), _types.CorrectionId(correction.value)))
 
 	def GetTabularCorrectionFactor(self, property: types.CorrectionProperty, correction: types.CorrectionId) -> OrthotropicTabularCorrectionFactor:
 		return OrthotropicTabularCorrectionFactor(self._Entity.GetTabularCorrectionFactor(_types.CorrectionProperty(property.value), _types.CorrectionId(correction.value)))
 
 	def Save(self) -> None:
+		'''
+		Save any changes to this orthotropic material to the database.
+		'''
 		return self._Entity.Save()
 
 
 class Vector2d:
+	'''
+	Represents a readonly 2D vector.
+	'''
 	def __init__(self, vector2d: _api.Vector2d):
 		self._Entity = vector2d
 
 	@property
 	def X(self) -> float:
 		return self._Entity.X
 
@@ -3077,30 +3404,40 @@
 		return self.Equals(other)
 
 	def __ne__(self, other):
 		return not self.Equals(other)
 
 
 class ElementSet(IdNameEntity):
+	'''
+	A set of elements defined in the input file.
+	'''
 	def __init__(self, elementSet: _api.ElementSet):
 		self._Entity = elementSet
 
 	@property
 	def Elements(self) -> ElementCol:
 		return ElementCol(self._Entity.Elements)
 
 
 class FemProperty(IdNameEntity):
+	'''
+	A property description.
+	'''
 	def __init__(self, femProperty: _api.FemProperty):
 		self._Entity = femProperty
 
 	@property
 	def Elements(self) -> ElementCol:
 		return ElementCol(self._Entity.Elements)
 
+	@property
+	def FemType(self) -> types.FemType:
+		return types.FemType[self._Entity.FemType.ToString()]
+
 
 class ElementSetCol(IdEntityCol[ElementSet]):
 	def __init__(self, elementSetCol: _api.ElementSetCol):
 		self._Entity = elementSetCol
 		self._CollectedClass = ElementSet
 
 	@property
@@ -3252,30 +3589,45 @@
 
 class SectionCut(IdNameEntity):
 	def __init__(self, sectionCut: _api.SectionCut):
 		self._Entity = sectionCut
 
 	@property
 	def ReferencePoint(self) -> types.SectionCutPropertyLocation:
+		'''
+		Centroid vs Origin
+		'''
 		return types.SectionCutPropertyLocation[self._Entity.ReferencePoint.ToString()]
 
 	@property
 	def HorizontalVector(self) -> Vector3d:
+		'''
+		Represents a readonly 3D vector.
+		'''
 		return Vector3d(self._Entity.HorizontalVector)
 
 	@property
 	def NormalVector(self) -> Vector3d:
+		'''
+		Represents a readonly 3D vector.
+		'''
 		return Vector3d(self._Entity.NormalVector)
 
 	@property
 	def OriginVector(self) -> Vector3d:
+		'''
+		Represents a readonly 3D vector.
+		'''
 		return Vector3d(self._Entity.OriginVector)
 
 	@property
 	def VerticalVector(self) -> Vector3d:
+		'''
+		Represents a readonly 3D vector.
+		'''
 		return Vector3d(self._Entity.VerticalVector)
 
 	@property
 	def MaxAngleBound(self) -> float:
 		return self._Entity.MaxAngleBound
 
 	@property
@@ -3328,22 +3680,31 @@
 
 	@property
 	def CQ_vmin(self) -> float:
 		return self._Entity.CQ_vmin
 
 	@property
 	def CG(self) -> Vector2d:
+		'''
+		Represents a readonly 2D vector.
+		'''
 		return Vector2d(self._Entity.CG)
 
 	@property
 	def CN(self) -> Vector2d:
+		'''
+		Represents a readonly 2D vector.
+		'''
 		return Vector2d(self._Entity.CN)
 
 	@property
 	def CQ(self) -> Vector2d:
+		'''
+		Represents a readonly 2D vector.
+		'''
 		return Vector2d(self._Entity.CQ)
 
 	@property
 	def EnclosedArea(self) -> float:
 		return self._Entity.EnclosedArea
 
 	@property
@@ -3451,17 +3812,23 @@
 		self._Entity.CQ_vmax = value
 
 	@CQ_vmin.setter
 	def CQ_vmin(self, value: float) -> None:
 		self._Entity.CQ_vmin = value
 
 	def AlignToHorizontalPrincipalAxes(self) -> None:
+		'''
+		Set this Section Cut's horizontal vector to be equal to its principal axis horizontal vector.
+		'''
 		return self._Entity.AlignToHorizontalPrincipalAxes()
 
 	def AlignToVerticalPrincipalAxes(self) -> None:
+		'''
+		Set this Section Cut's horizontal vector to be equal to its principal axis vertical vector.
+		'''
 		return self._Entity.AlignToVerticalPrincipalAxes()
 
 	def SetHorizontalVector(self, vector: Vector3d) -> None:
 		return self._Entity.SetHorizontalVector(vector._Entity)
 
 	def SetNormalVector(self, vector: Vector3d) -> None:
 		return self._Entity.SetNormalVector(vector._Entity)
@@ -3653,14 +4020,17 @@
 	def PlyColList(self) -> tuple[Ply]:
 		return tuple([Ply(plyCol) for plyCol in self._Entity])
 
 	def Delete(self, id: int) -> CollectionModificationStatus:
 		return CollectionModificationStatus[self._Entity.Delete(id).ToString()]
 
 	def DeleteAll(self) -> None:
+		'''
+		Delete all plies in the collection.
+		'''
 		return self._Entity.DeleteAll()
 
 	def ExportToCSV(self, filepath: str) -> None:
 		return self._Entity.ExportToCSV(filepath)
 
 	def ImportCSV(self, filepath: str) -> None:
 		return self._Entity.ImportCSV(filepath)
@@ -3734,15 +4104,18 @@
 
 	def CreateZone(self, elementIds: tuple[int], name: str = None) -> None:
 		elementIdsList = MakeCSharpIntList(elementIds)
 		elementIdsEnumerable = IEnumerable(elementIdsList)
 		return self._Entity.CreateZone(elementIdsEnumerable, name)
 
 	def CreatePanelSegment(self, discreteTechnique: types.DiscreteTechnique, discreteElementLkp: dict[types.DiscreteDefinitionType, list[int]], name: str = None) -> int:
-		return self._Entity.CreatePanelSegment(_types.DiscreteTechnique(discreteTechnique.value), discreteElementLkp._Entity, name)
+		discreteElementLkpDict = Dictionary[_types.DiscreteDefinitionType, List[int]]()
+		for kvp in discreteElementLkp:
+			discreteElementLkpDict.Add(_types.DiscreteDefinitionType(kvp.value), MakeCSharpIntList(discreteElementLkp[kvp]))
+		return self._Entity.CreatePanelSegment(_types.DiscreteTechnique(discreteTechnique.value), discreteElementLkpDict, name)
 
 	@overload
 	def Remove(self, zoneIds: tuple[int], jointIds: tuple[int]) -> CollectionModificationStatus: ...
 
 	@overload
 	def Remove(self, zoneIds: tuple[int], jointIds: tuple[int], panelSegmentIds: tuple[int]) -> CollectionModificationStatus: ...
 
@@ -4030,22 +4403,22 @@
 	def __iter__(self):
 		yield from self.DesignLoadColList
 
 	def __len__(self):
 		return len(self.DesignLoadColList)
 
 
-class DiscreteFieldTableCol(IdNameEntityCol[DiscreteFieldTable]):
-	def __init__(self, discreteFieldTableCol: _api.DiscreteFieldTableCol):
-		self._Entity = discreteFieldTableCol
-		self._CollectedClass = DiscreteFieldTable
+class DiscreteFieldCol(IdNameEntityCol[DiscreteField]):
+	def __init__(self, discreteFieldCol: _api.DiscreteFieldCol):
+		self._Entity = discreteFieldCol
+		self._CollectedClass = DiscreteField
 
 	@property
-	def DiscreteFieldTableColList(self) -> tuple[DiscreteFieldTable]:
-		return tuple([DiscreteFieldTable(discreteFieldTableCol) for discreteFieldTableCol in self._Entity])
+	def DiscreteFieldColList(self) -> tuple[DiscreteField]:
+		return tuple([DiscreteField(discreteFieldCol) for discreteFieldCol in self._Entity])
 
 	def Create(self, name: str, entityType: types.DiscreteFieldPhysicalEntityType, dataType: types.DiscreteFieldDataType) -> int:
 		return self._Entity.Create(name, _types.DiscreteFieldPhysicalEntityType(entityType.value), _types.DiscreteFieldDataType(dataType.value))
 
 	def CreateFromVCP(self, filepath: str) -> list[int]:
 		return list[int](self._Entity.CreateFromVCP(filepath))
 
@@ -4054,36 +4427,36 @@
 
 	def CreateByPointMapToElements(self, elementIds: list[int], discreteFieldIds: list[int], suffix: str = None, tolerance: float = None) -> None:
 		elementIdsList = MakeCSharpIntList(elementIds)
 		discreteFieldIdsList = MakeCSharpIntList(discreteFieldIds)
 		return self._Entity.CreateByPointMapToElements(elementIdsList, discreteFieldIdsList, suffix, tolerance)
 
 	@overload
-	def Get(self, name: str) -> DiscreteFieldTable: ...
+	def Get(self, name: str) -> DiscreteField: ...
 
 	@overload
-	def Get(self, id: int) -> DiscreteFieldTable: ...
+	def Get(self, id: int) -> DiscreteField: ...
 
-	def Get(self, item1 = None) -> DiscreteFieldTable:
+	def Get(self, item1 = None) -> DiscreteField:
 		if isinstance(item1, str):
-			return DiscreteFieldTable(super().Get(item1))
+			return DiscreteField(super().Get(item1))
 
 		if isinstance(item1, int):
-			return DiscreteFieldTable(super().Get(item1))
+			return DiscreteField(super().Get(item1))
 
 		return self._Entity.Get(item1)
 
 	def __getitem__(self, index: int):
-		return self.DiscreteFieldTableColList[index]
+		return self.DiscreteFieldColList[index]
 
 	def __iter__(self):
-		yield from self.DiscreteFieldTableColList
+		yield from self.DiscreteFieldColList
 
 	def __len__(self):
-		return len(self.DiscreteFieldTableColList)
+		return len(self.DiscreteFieldColList)
 
 
 class ZoneJointContainerCol(IdNameEntityCol, Generic[T]):
 	def __init__(self, zoneJointContainerCol: _api.ZoneJointContainerCol):
 		self._Entity = zoneJointContainerCol
 		self._CollectedClass = T
 
@@ -4099,18 +4472,18 @@
 	def Get(self, name: str) -> T: ...
 
 	@overload
 	def Get(self, id: int) -> T: ...
 
 	def Get(self, item1 = None) -> T:
 		if isinstance(item1, str):
-			return T(super().Get(item1))
+			return super().Get(item1)
 
 		if isinstance(item1, int):
-			return T(super().Get(item1))
+			return super().Get(item1)
 
 		return self._Entity.Get(item1)
 
 	def __getitem__(self, index: int):
 		return self.ZoneJointContainerColList[index]
 
 	def __iter__(self):
@@ -4274,14 +4647,17 @@
 		yield from self.StructureColList
 
 	def __len__(self):
 		return len(self.StructureColList)
 
 
 class Project:
+	'''
+	Represents a HyperX project within a database.
+	'''
 	def __init__(self, project: _api.Project):
 		self._Entity = project
 
 	@property
 	def WorkingFolder(self) -> str:
 		return self._Entity.WorkingFolder
 
@@ -4334,16 +4710,16 @@
 		return SectionCutCol(self._Entity.SectionCuts)
 
 	@property
 	def DesignLoads(self) -> DesignLoadCol:
 		return DesignLoadCol(self._Entity.DesignLoads)
 
 	@property
-	def DiscreteFieldTables(self) -> DiscreteFieldTableCol:
-		return DiscreteFieldTableCol(self._Entity.DiscreteFieldTables)
+	def DiscreteFieldTables(self) -> DiscreteFieldCol:
+		return DiscreteFieldCol(self._Entity.DiscreteFieldTables)
 
 	@property
 	def AnalysisProperties(self) -> AnalysisPropertyCol:
 		return AnalysisPropertyCol(self._Entity.AnalysisProperties)
 
 	@property
 	def DesignProperties(self) -> DesignPropertyCol:
@@ -4362,14 +4738,18 @@
 		if tags is not None:
 			for thing in tags:
 				if thing is not None:
 					tagsList.Add(thing)
 		return self._Entity.Upload(uploadSetName, company, program, tagsList, notes, zoneIds._Entity, jointIds._Entity)
 
 	def GetDashboardCompanies(self) -> list[str]:
+		'''
+		This method fetches an array of Dashboard company names that are available to the user who is currently logged in. The URL and authentication token are taken from the last
+            Dashboard login made through HyperX.
+		'''
 		return list[str](self._Entity.GetDashboardCompanies())
 
 	def GetDashboardPrograms(self, companyName: str) -> list[str]:
 		return list[str](self._Entity.GetDashboardPrograms(companyName))
 
 	def GetDashboardTags(self, companyName: str) -> list[str]:
 		return list[str](self._Entity.GetDashboardTags(companyName))
@@ -4712,23 +5092,38 @@
 		yield from self.ProjectInfoColList
 
 	def __len__(self):
 		return len(self.ProjectInfoColList)
 
 
 class Application:
+	'''
+	HyperX scripting application.
+            This API is not guaranteed to be thread-safe.
+            Calls into a single application instance or its descendents are not safe to be called concurrently.
+            
+            However, it is safe enough for integration testing to have multiple
+            application instances with a single process.
+	'''
 	def __init__(self, application: _api.Application):
 		self._Entity = application
 
 	@property
+	def CompilationDate(self) -> str:
+		return self._Entity.CompilationDate
+
+	@property
 	def DatabasePath(self) -> str:
 		return self._Entity.DatabasePath
 
 	@property
 	def ActiveProject(self) -> Project:
+		'''
+		Represents a HyperX project within a database.
+		'''
 		return Project(self._Entity.ActiveProject)
 
 	@property
 	def UiRunnerMode(self) -> bool:
 		return self._Entity.UiRunnerMode
 
 	@property
@@ -4741,22 +5136,31 @@
 
 	@property
 	def FailureModes(self) -> FailureModeCol:
 		return FailureModeCol(self._Entity.FailureModes)
 
 	@property
 	def Foams(self) -> FoamCol:
+		'''
+		Contains a set of all foam materials in a database.
+		'''
 		return FoamCol(self._Entity.Foams)
 
 	@property
 	def Honeycombs(self) -> HoneycombCol:
+		'''
+		Contains a set of all honeycomb materials in a database.
+		'''
 		return HoneycombCol(self._Entity.Honeycombs)
 
 	@property
 	def Isotropics(self) -> IsotropicCol:
+		'''
+		Contains a set of all isotropic materials in a database.
+		'''
 		return IsotropicCol(self._Entity.Isotropics)
 
 	@property
 	def AnalysisProperties(self) -> AnalysisPropertyCol:
 		return AnalysisPropertyCol(self._Entity.AnalysisProperties)
 
 	@property
@@ -4765,18 +5169,24 @@
 
 	@property
 	def LoadProperties(self) -> LoadPropertyCol:
 		return LoadPropertyCol(self._Entity.LoadProperties)
 
 	@property
 	def Orthotropics(self) -> OrthotropicCol:
+		'''
+		Contains a set of all orthotropic materials in a database.
+		'''
 		return OrthotropicCol(self._Entity.Orthotropics)
 
 	@property
 	def ProjectInfos(self) -> ProjectInfoCol:
+		'''
+		Contains a set of all projects in a database.
+		'''
 		return ProjectInfoCol(self._Entity.ProjectInfos)
 
 	@property
 	def UserName(self) -> str:
 		return self._Entity.UserName
 
 	@UserName.setter
@@ -4804,17 +5214,24 @@
 	def DeleteAnalysisProperty(self, id: int) -> None:
 		return self._Entity.DeleteAnalysisProperty(id)
 
 	def DeleteProject(self, projectName: str) -> ProjectDeletionStatus:
 		return ProjectDeletionStatus[self._Entity.DeleteProject(projectName).ToString()]
 
 	def Dispose(self) -> None:
+		'''
+		Dispose of the application. Should be explicitly called after the application
+            is no longer needed unless the application is wrapped with a using clause.
+		'''
 		return self._Entity.Dispose()
 
 	def GetAnalyses(self) -> dict[int, AnalysisDefinition]:
+		'''
+		Get all Analysis Defintions in the database.
+		'''
 		return dict[int, AnalysisDefinition](self._Entity.GetAnalyses())
 
 	def Login(self, userName: str, password: str = "") -> None:
 		return self._Entity.Login(userName, password)
 
 	def Migrate(self, databasePath: str) -> str:
 		return self._Entity.Migrate(databasePath)
@@ -4828,14 +5245,17 @@
 
 class JointDesignProperty(DesignProperty):
 	def __init__(self, jointDesignProperty: _api.JointDesignProperty):
 		self._Entity = jointDesignProperty
 
 
 class ToolingConstraint(IdNameEntity):
+	'''
+	Tooling constraints are a feature of Design Properties for Zones.
+	'''
 	def __init__(self, toolingConstraint: _api.ToolingConstraint):
 		self._Entity = toolingConstraint
 
 	@property
 	def ConstraintMax(self) -> float:
 		return self._Entity.ConstraintMax
 
@@ -4845,14 +5265,17 @@
 
 	@property
 	def ConstraintValue(self) -> float:
 		return self._Entity.ConstraintValue
 
 	@property
 	def ToolingSelectionType(self) -> types.ToolingSelectionType:
+		'''
+		Defines which selection a given tooling constraint is currently set to.
+		'''
 		return types.ToolingSelectionType[self._Entity.ToolingSelectionType.ToString()]
 
 	def SetToAnyValue(self) -> None:
 		return self._Entity.SetToAnyValue()
 
 	def SetToInequality(self, value: float) -> None:
 		return self._Entity.SetToInequality(value)
@@ -4861,14 +5284,18 @@
 		return self._Entity.SetToRange(min, max)
 
 	def SetToValue(self, value: float) -> None:
 		return self._Entity.SetToValue(value)
 
 
 class DesignVariable(IdEntity):
+	'''
+	Holds design variable data.
+            Min, max, steps, materials.
+	'''
 	def __init__(self, designVariable: _api.DesignVariable):
 		self._Entity = designVariable
 
 	@property
 	def AllowMaterials(self) -> bool:
 		return self._Entity.AllowMaterials
 
@@ -4909,25 +5336,34 @@
 		self._Entity.UseAnalysis = value
 
 	def AddMaterials(self, materialIds: list[int]) -> None:
 		materialIdsList = MakeCSharpIntList(materialIds)
 		return self._Entity.AddMaterials(materialIdsList)
 
 	def GetSizingMaterials(self) -> list[int]:
+		'''
+		Get a list of materials used for sizing, if they exist.
+		'''
 		return list[int](self._Entity.GetSizingMaterials())
 
 	def GetAnalysisMaterial(self) -> int:
+		'''
+		Get the material used for analysis, if it exists.
+		'''
 		return self._Entity.GetAnalysisMaterial()
 
 	def RemoveSizingMaterials(self, materialIds: tuple[int] = None) -> None:
 		materialIdsList = MakeCSharpIntList(materialIds)
 		materialIdsEnumerable = IEnumerable(materialIdsList)
 		return self._Entity.RemoveSizingMaterials(materialIds if materialIds is None else materialIdsEnumerable)
 
 	def RemoveAnalysisMaterial(self) -> None:
+		'''
+		Remove the analysis material assigned to this variable.
+		'''
 		return self._Entity.RemoveAnalysisMaterial()
 
 
 class ToolingConstraintCol(IdNameEntityCol[ToolingConstraint]):
 	def __init__(self, toolingConstraintCol: _api.ToolingConstraintCol):
 		self._Entity = toolingConstraintCol
 		self._CollectedClass = ToolingConstraint
@@ -4990,108 +5426,54 @@
 
 	@property
 	def DesignVariables(self) -> DesignVariableCol:
 		return DesignVariableCol(self._Entity.DesignVariables)
 
 
 class Environment(ABC):
+	'''
+	Represents HyperX's execution environment (where HyperX is installed).
+	'''
 	def __init__(self, environment: _api.Environment):
 		self._Entity = environment
 
 	def SetLocation(self, location: str) -> None:
 		return self._Entity.SetLocation(location)
 
 	def Initialize(self) -> None:
+		'''
+		Initialize the HyperX scripting environment.
+		'''
 		return self._Entity.Initialize()
 
 
 class FailureCriterionSetting(FailureSetting):
+	'''
+	Setting for a Failure Criteria.
+	'''
 	def __init__(self, failureCriterionSetting: _api.FailureCriterionSetting):
 		self._Entity = failureCriterionSetting
 
 
 class FailureModeSetting(FailureSetting):
+	'''
+	Setting for a Failure Mode.
+	'''
 	def __init__(self, failureModeSetting: _api.FailureModeSetting):
 		self._Entity = failureModeSetting
 
 
 class HelperFunctions(ABC):
 	def __init__(self, helperFunctions: _api.HelperFunctions):
 		self._Entity = helperFunctions
 
 	def NullableSingle(self, input: float) -> float:
 		return self._Entity.NullableSingle(input)
 
 
-class TabularCorrectionFactorIndependentValue:
-	def __init__(self, tabularCorrectionFactorIndependentValue: _api.TabularCorrectionFactorIndependentValue):
-		self._Entity = tabularCorrectionFactorIndependentValue
-
-	@property
-	def BoolValue(self) -> bool:
-		return self._Entity.BoolValue
-
-	@property
-	def DoubleValue(self) -> float:
-		return self._Entity.DoubleValue
-
-	@property
-	def IntValue(self) -> int:
-		return self._Entity.IntValue
-
-	@property
-	def ValueType(self) -> types.CorrectionValueType:
-		return types.CorrectionValueType[self._Entity.ValueType.ToString()]
-
-
-class OrthotropicEffectiveLaminate:
-	def __init__(self, orthotropicEffectiveLaminate: _api.OrthotropicEffectiveLaminate):
-		self._Entity = orthotropicEffectiveLaminate
-
-	@property
-	def Percent_tape_0(self) -> float:
-		return self._Entity.Percent_tape_0
-
-	@property
-	def Percent_tape_90(self) -> float:
-		return self._Entity.Percent_tape_90
-
-	@property
-	def Percent_tape_45(self) -> float:
-		return self._Entity.Percent_tape_45
-
-	@property
-	def Percent_fabric_0(self) -> float:
-		return self._Entity.Percent_fabric_0
-
-	@property
-	def Percent_fabric_90(self) -> float:
-		return self._Entity.Percent_fabric_90
-
-	@property
-	def Percent_fabric_45(self) -> float:
-		return self._Entity.Percent_fabric_45
-
-	@property
-	def Tape_Orthotropic(self) -> str:
-		return self._Entity.Tape_Orthotropic
-
-	@property
-	def Fabric_Orthotropic(self) -> str:
-		return self._Entity.Fabric_Orthotropic
-
-	@property
-	def Valid(self) -> bool:
-		return self._Entity.Valid
-
-	@property
-	def Use_tape_allowables(self) -> bool:
-		return self._Entity.Use_tape_allowables
-
-
 class Beam(Zone):
 	def __init__(self, beam: _api.Beam):
 		self._Entity = beam
 
 	@property
 	def Length(self) -> float:
 		return self._Entity.Length
```

### Comparing `hyperx-0.1.2/hyperx/library/find.py` & `hyperx-0.1.6/hyperx/library/find.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.2/hyperx/library/library.py` & `hyperx-0.1.6/hyperx/library/library.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.2/hyperx/utils/utils.py` & `hyperx-0.1.6/hyperx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.2/hyperx.egg-info/PKG-INFO` & `hyperx-0.1.6/hyperx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.2
+Version: 0.1.6
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.2/pyproject.toml` & `hyperx-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hyperx"
-version = "0.1.2"
+version = "0.1.6"
 authors = [
   { name="Kelly Ann Smith", email="kellyann.smith@collieraerospace.com" },
   { name="Noah Prezant", email="noah.prezant@collieraerospace.com" },
 ]
 description = "HyperX scripting for Python"
 readme = "README.md"
 requires-python = ">=3.10"
```

